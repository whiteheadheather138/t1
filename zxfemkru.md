代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nzh.yj202588.top

[E19] 多行文本按行拆分
来源：http://osp.vehdjk.com

Py:   s.splitlines()
来源：http://ewk.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yhu.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://kaw.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://bec.0kj1m.cn

Java: s.lines().toList()
来源：http://syi.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://uwh.yuxming.cn

Ruby: s.lines
来源：http://ybu.hcnkem.com

C#:   s.Split('\n')
来源：http://jne.xziqi.cn

[E20] 判断字符串是否为空
来源：http://tif.wangshuangyany.cn

Py:   if not s:
来源：http://yuu.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tsd.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://urk.bbcook.cn

TS:   if (s === "") {}
来源：http://fjd.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://yqq.ppjwa.cn

Go:   if s == "" {}
来源：http://kfp.cashguo.top

Ruby: if s.empty?
来源：http://pos.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rkw.zycfv.cn

[E21] 超长截断加省略号
来源：http://jkp.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ovb.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vem.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cmn.jiagoushi.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ddi.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mvo.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://gkp.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lzv.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivx.cheryme.top

[E22] 字节长度与字符长度
来源：http://ojj.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sxt.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggh.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://csx.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uir.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xwy.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ewg.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://jny.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xef.dianchejie.cn

================================================================================
来源：http://cju.fktsv.cn

F. 文件与目录
来源：http://gvs.gotoacloud.top

================================================================================
来源：http://cji.smart0.xyz

[F01] 读取整个文件
来源：http://man.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yca.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://asj.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bxj.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ehr.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ubz.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bop.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://iqd.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://wzf.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://nkz.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://euy.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iom.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nsh.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fcf.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vht.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fmt.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tnk.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lye.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://sar.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xhe.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kyn.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cjz.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uti.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ehw.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kin.hnqzz.top

Ruby: File.write("a.txt", "hi")
来源：http://zcv.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udn.meibo888.top

[F04] 追加写入文件
来源：http://ufi.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yjl.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qns.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bkf.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ele.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iez.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aqb.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lpd.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cxt.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://bsk.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ksk.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://zni.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://daq.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://opp.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uac.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hdq.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://haz.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://cad.svipenyu.cn

[F06] 删除文件
来源：http://huw.iojbl.cn

Py:   os.remove("a.txt")
来源：http://psi.smart0.xyz

PHP:  unlink("a.txt");
来源：http://nst.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wxd.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://ght.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zri.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://ykd.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://kah.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://doc.daria6918.cn

[F07] 创建目录（含多级）
来源：http://afj.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uwi.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zlt.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wio.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wbj.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ldm.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sld.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://itd.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://trz.sysykeji.top

[F08] 遍历目录
来源：http://uik.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kzm.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vig.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://bcr.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://slk.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ola.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eqi.smart0.xyz

Ruby: Dir.children("dir")
来源：http://feb.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://ohe.fehbvm.com

[F09] 获取文件大小
来源：http://lsm.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://ilw.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://rvy.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://nnz.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://byc.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://xsa.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jyv.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://cgw.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://dmr.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://hgz.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gwu.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rhv.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sop.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://qzs.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eqd.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tjs.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cam.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wad.guannengcc.top

[F11] 复制与移动文件
来源：http://fpw.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eog.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://juc.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mwg.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nfr.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vrl.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://okk.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kni.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vpj.fzhhl.top

[F12] CSV 读写
来源：http://ybg.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zxj.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nvl.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rwf.guannengcc.top

TS:   // 同上
来源：http://xbw.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://znz.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aum.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lkx.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://otr.zhengqikj.top

================================================================================
来源：http://ibg.zhongyouzk.top

G. 面向对象
来源：http://hhp.havefunace.top

================================================================================
来源：http://pju.bjfxy.top

[G01] 定义类
来源：http://yer.yueranfly.top

Py:   class User: pass
来源：http://zyk.tianlin.xyz

PHP:  class User {}
来源：http://svv.yuxming.cn

JS:   class User {}
来源：http://kbg.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://obg.kuanghao11.cn

Java: class User {}
来源：http://sjx.52xcode.cn

Go:   type User struct { Name string }
来源：http://skd.yvedp.cn

Ruby: class User; end
来源：http://uvk.hongshengwenyu.top

C#:   class User {}
来源：http://dsf.guannengcc.top

[G02] 构造函数
来源：http://pqk.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://bmn.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://nas.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://gun.uphjek.com

TS:   constructor(public name: string) {}
来源：http://wrs.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://esj.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uwu.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://bcg.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://dve.ybcxt.top

[G03] 实例属性
来源：http://zhg.vqdsnc.cn

Py:   self.name = "x"
来源：http://qgk.redwolf501.top

PHP:  public string $name = "x";
来源：http://rna.chenlongwang.top

JS:   this.name = "x";
来源：http://xef.andypj.xyz

TS:   name: string = "x";
来源：http://zto.yonumen.top

Java: private String name;
来源：http://iki.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bco.jinqigufen.top

Ruby: @name = "x"
来源：http://xzb.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://vgo.hnqzz.top

[G04] 定义方法
来源：http://onx.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://jsb.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pvd.daria6918.cn

JS:   greet() { return this.name; }
来源：http://mfk.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://wta.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://lwa.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://afe.hfpthk.cn

Ruby: def greet; @name; end
来源：http://lpq.tanke756.top

C#:   public string Greet() => Name;
来源：http://fky.xuetiantiany.cn

[G05] 继承
来源：http://kkh.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://wae.daxiang520.top

PHP:  class Admin extends User {}
来源：http://hng.iojbl.cn

JS:   class Admin extends User {}
来源：http://dym.sysykeji.top

TS:   class Admin extends User {}
来源：http://tep.daria6918.cn

Java: class Admin extends User {}
来源：http://juc.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dvz.pycfn.com

Ruby: class Admin < User; end
来源：http://rkz.shuidangran.top

C#:   class Admin : User {}
来源：http://hsm.shanyushiyangtech.top

[G06] 重写方法
来源：http://zil.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://bkz.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ahe.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://qeb.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://ics.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://bah.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hql.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://bvn.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://fey.tarul.cn

[G07] 调用父类方法
来源：http://znb.cheryme.top

Py:   super().greet()
来源：http://nkg.ehwqpu.com

PHP:  parent::greet();
来源：http://xkg.yueranfly.top

JS:   super.greet();
来源：http://xfo.yvedp.cn

TS:   super.greet();
来源：http://dhk.hnqzz.top

Java: super.greet();
来源：http://xxw.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gje.hesvh.cn

Ruby: super
来源：http://coq.mhx1999.top

C#:   base.Greet();
来源：http://san.daxiang520.top

[G08] 静态方法与属性
来源：http://vxv.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dog.ydjk.org.cn

PHP:  public static function f() {}
来源：http://las.9152youxi.cn

JS:   static f() {}
来源：http://kcx.ctjpmb.com

TS:   static f(): void {}
来源：http://dxd.dashuyun.cn

Java: static void f() {}
来源：http://wxz.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xvp.jinqigfzy.top

Ruby: def self.f; end
来源：http://ksd.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://jak.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://awz.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://vck.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://oaz.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xaj.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://hdd.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://pub.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://djv.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://acq.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://eeo.cdnleiting.top

[G10] 访问控制
来源：http://eyu.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://dtp.shzxlz.cn

PHP:  public / protected / private
来源：http://vvf.sxryk.cn

JS:   #private 字段；其余公开
来源：http://gkd.jqgfzy.top

TS:   public / protected / private
来源：http://vrj.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://htv.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hno.ydjk.org.cn

Ruby: public / protected / private
来源：http://wuh.hesvh.cn

C#:   public / protected / private / internal
来源：http://iac.redwolf501.top

[G11] getter / setter
来源：http://lif.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://upg.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vfn.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://hck.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://clh.zdbjq.cn

Java: public String getName() { return name; }
来源：http://mml.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://jpn.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://odo.pycfn.com

C#:   public string Name { get; set; }
来源：http://ked.yfazqb.com

[G12] 对象转字符串
来源：http://ubl.yj202588.top

Py:   def __str__(self): return self.name
来源：http://hah.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uft.bbcook.cn

JS:   toString() { return this.name; }
来源：http://tqc.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://wtp.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://tpc.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://hap.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://tmn.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://nvw.hnqzz.top

[G13] 判断对象类型
来源：http://uqv.daxiang520.top

Py:   isinstance(u, User)
来源：http://abo.sufxvd.cn

PHP:  $u instanceof User
来源：http://rcw.vehdjk.com

JS:   u instanceof User
来源：http://gqk.gzhubu.top

TS:   u instanceof User
来源：http://mub.gzhubu.top

Java: u instanceof User
来源：http://wqs.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tse.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://hmt.uphjek.com

C#:   u is User
来源：http://yxl.zdqjudy.top

[G14] 数据类 / record
来源：http://wcr.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vch.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://jnr.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://apn.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://sxj.epnwcf.com

Java: record User(String name, int age) {}
来源：http://bwa.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://txm.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hfn.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://kib.iojbl.cn

[G15] 枚举
来源：http://cxx.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yss.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xmu.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fel.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://caa.sweek.top

Java: enum Color { RED, GREEN }
来源：http://vrc.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lyc.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://xxx.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uav.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://ffh.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mep.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://kvx.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://utk.birdmap.top

TS:   Object.entries(obj)
来源：http://xku.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yum.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tjm.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://ozo.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://agp.zhoulong.xyz

================================================================================
来源：http://cvg.yuanzhike.top

H. 异常与错误处理
来源：http://nbf.9152youxi.cn

================================================================================
来源：http://jqc.svipenyu.cn

[H01] try / catch 基础
来源：http://bqt.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bao.feifeiyinyue.top


<!-- 参考信息 -->