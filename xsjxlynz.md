代发 wailian999

Ruby: s.lines
来源：http://nua.sysykeji.top

C#:   s.Split('\n')
来源：http://vxf.sysykeji.top

[E20] 判断字符串是否为空
来源：http://rev.cucudq.cn

Py:   if not s:
来源：http://cdo.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tnk.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxo.pycfn.com

TS:   if (s === "") {}
来源：http://bam.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://dkt.ivvv.top

Go:   if s == "" {}
来源：http://sww.tanke756.top

Ruby: if s.empty?
来源：http://pms.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cdj.hcnkem.com

[E21] 超长截断加省略号
来源：http://xom.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lqi.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpe.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://siw.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szk.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hvq.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://pil.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://psj.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nhu.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://dwi.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ddr.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvg.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://joy.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gul.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dxp.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ycv.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://dqo.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gnf.tanke756.top

================================================================================
来源：http://wcx.shanyushiyangkeji.top

F. 文件与目录
来源：http://pod.fehbvm.com

================================================================================
来源：http://rbm.tanke756.top

[F01] 读取整个文件
来源：http://xxt.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pni.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://gyc.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vcq.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uug.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjm.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kaa.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://gup.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://bpt.jyoumei.cn

[F02] 逐行读取文件
来源：http://yjd.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wkq.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qqk.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ivj.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://djl.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nym.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nro.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kse.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rzo.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://mvc.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kpq.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://urw.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xov.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rse.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ktm.cashguo.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ypp.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ngx.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vqs.0kj1m.cn

[F04] 追加写入文件
来源：http://btk.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lfm.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hmy.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iyn.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://saa.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hgk.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hvg.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hms.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vdl.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://jtp.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uqq.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://dtn.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://ayd.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://fjl.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xgg.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ish.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://ygf.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://tqp.gaohongyu789.top

[F06] 删除文件
来源：http://zto.daria6918.cn

Py:   os.remove("a.txt")
来源：http://lze.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://jpj.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://stz.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fvo.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://onh.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://pab.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://orf.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://sxq.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://ojs.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rsy.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://czz.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://emz.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dtv.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uec.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://esk.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zrr.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bjd.hongshengwenyu.top

[F08] 遍历目录
来源：http://ttn.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://smc.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zpe.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://die.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://edu.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wsa.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://liw.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://njx.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://pol.shzxlz.cn

[F09] 获取文件大小
来源：http://ibn.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://jst.tanke756.top

PHP:  filesize("a.txt");
来源：http://scp.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://fxf.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://njg.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://fvg.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://swm.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://zim.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://xmu.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://zml.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mii.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://abd.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fnw.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://pnu.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sbm.52xcode.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cyz.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://obj.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://flr.mhx1999.top

[F11] 复制与移动文件
来源：http://vcx.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bqg.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ism.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjg.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pay.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cqo.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uxx.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mzc.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://csp.yongpay.top

[F12] CSV 读写
来源：http://cta.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fkj.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hvv.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dgq.ppjwa.cn

TS:   // 同上
来源：http://flp.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mpj.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xaj.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ved.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://yql.wangdashe.top

================================================================================
来源：http://xyf.hywenlv.cn

G. 面向对象
来源：http://uag.pengpengdd.cyou

================================================================================
来源：http://lpq.wangdashe.top

[G01] 定义类
来源：http://nod.xuetiantiany.cn

Py:   class User: pass
来源：http://nhq.sysykeji.top

PHP:  class User {}
来源：http://dxz.chenlongwang.top

JS:   class User {}
来源：http://caq.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://xoy.zhijiandao.cn

Java: class User {}
来源：http://ndn.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://vcd.kuanghao11.cn

Ruby: class User; end
来源：http://bct.meibo888.top

C#:   class User {}
来源：http://vxy.ybcxt.top

[G02] 构造函数
来源：http://azl.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://ydn.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://wqo.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://jyr.yonumen.top

TS:   constructor(public name: string) {}
来源：http://xvn.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://isc.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bnc.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://ijq.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://eri.bbcook.cn

[G03] 实例属性
来源：http://zyj.nanxinkj.top

Py:   self.name = "x"
来源：http://lkb.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://jqa.xinyue.icu

JS:   this.name = "x";
来源：http://xfu.jinqigufen.top

TS:   name: string = "x";
来源：http://pmw.316326.xyz

Java: private String name;
来源：http://fvu.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qxr.fehbvm.com

Ruby: @name = "x"
来源：http://iap.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://nyg.cqqwz.cn

[G04] 定义方法
来源：http://rzy.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://ywg.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zyg.316326.xyz

JS:   greet() { return this.name; }
来源：http://fhz.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://imu.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://ymc.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xje.sysykeji.top

Ruby: def greet; @name; end
来源：http://xzz.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://lxn.yj20258888.top

[G05] 继承
来源：http://eir.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://hah.cheryme.top

PHP:  class Admin extends User {}
来源：http://zki.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://hsy.yuxming.cn

TS:   class Admin extends User {}
来源：http://yyg.vehdjk.com

Java: class Admin extends User {}
来源：http://lgz.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fha.zycfv.cn

Ruby: class Admin < User; end
来源：http://xgm.gotoacloud.top

C#:   class Admin : User {}
来源：http://kmg.aibaodan.cn

[G06] 重写方法
来源：http://zhe.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://end.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bam.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://juk.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://hba.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://vjz.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ccx.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://lfr.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://zkm.birdmap.top

[G07] 调用父类方法
来源：http://bte.cheryme.top

Py:   super().greet()
来源：http://nhk.guannengcc.top

PHP:  parent::greet();
来源：http://zht.sufxvd.cn

JS:   super.greet();
来源：http://nij.sjlbkw.cn

TS:   super.greet();
来源：http://atw.chenlongwang.top

Java: super.greet();
来源：http://jaz.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://syn.yj20258.top

Ruby: super
来源：http://ihd.hesvh.cn

C#:   base.Greet();
来源：http://yqj.cucudq.cn

[G08] 静态方法与属性
来源：http://unm.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cjz.chenzaomai.com

PHP:  public static function f() {}
来源：http://kpx.guowangkeji.top

JS:   static f() {}
来源：http://tjp.ehwqpu.com

TS:   static f(): void {}
来源：http://heg.jlsjyb.cn

Java: static void f() {}
来源：http://hqd.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ujs.havefunace.top

Ruby: def self.f; end
来源：http://pym.gaohongyu789.top

C#:   public static void F() {}
来源：http://umr.yvedp.cn

[G09] 接口 / 抽象类
来源：http://irc.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://kmt.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://enh.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mqi.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://jsn.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://fvt.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://jgp.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pxa.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://ppn.shuidangran.top

[G10] 访问控制
来源：http://ddl.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://xok.jiagoushi.top

PHP:  public / protected / private
来源：http://aob.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://ehu.jyoumei.cn

TS:   public / protected / private
来源：http://qzd.sweek.top

Java: public / protected / private / 默认包级
来源：http://zid.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tmt.wangshuangyany.cn

Ruby: public / protected / private
来源：http://zng.chenzaomai.com

C#:   public / protected / private / internal
来源：http://yul.guannengcc.top

[G11] getter / setter
来源：http://cka.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://iha.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aca.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://edq.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://wok.fzhhl.top

Java: public String getName() { return name; }
来源：http://ijv.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://mto.aibaodan.cn

Ruby: attr_accessor :name
来源：http://obz.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://tbn.gzhubu.top

[G12] 对象转字符串
来源：http://rph.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://ely.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://huo.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://bmb.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://ikk.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://tqn.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://ybc.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://jnw.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://mos.sweek.top

[G13] 判断对象类型
来源：http://qwc.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://avf.mhx1999.top

PHP:  $u instanceof User
来源：http://syi.uphjek.com

JS:   u instanceof User
来源：http://mzp.cdnleiting.top

TS:   u instanceof User
来源：http://rsk.tianlin.xyz

Java: u instanceof User
来源：http://kfj.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lvc.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://gob.haohaochexian.top

C#:   u is User
来源：http://lyl.feifeiyinyue.top

[G14] 数据类 / record
来源：http://egk.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cvt.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://crr.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://isb.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://hsz.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://yfa.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://qtn.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gmu.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://tfv.yanxiufei.cn

[G15] 枚举
来源：http://yai.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zqb.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hat.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wzl.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zls.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://bge.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bdx.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://wge.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ypv.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://ngq.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jho.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://vmn.yj20258888.top

JS:   Object.entries(obj)
来源：http://fvk.ppjwa.cn

TS:   Object.entries(obj)
来源：http://zyr.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ehm.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://mzk.yvedp.cn

Ruby: obj.instance_variables
来源：http://rnk.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://waz.jinyuanbaomall.cn

================================================================================
来源：http://sca.shangyingyoupin.top

H. 异常与错误处理
来源：http://ikk.zhixingplan.top

================================================================================
来源：http://ktu.zhiwuduotai.top

[H01] try / catch 基础
来源：http://ycb.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wby.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mwd.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zoc.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://krl.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oue.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qzd.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uic.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xjj.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://chh.hammf.cn


<!-- 参考信息 -->