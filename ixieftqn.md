代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iug.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ukm.hywenlv.cn

TS:   if (s === "") {}
来源：http://zcy.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://nyu.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://kqe.hesvh.cn

Ruby: if s.empty?
来源：http://vnp.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://huq.gzhubu.top

[E21] 超长截断加省略号
来源：http://ayz.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xso.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ryz.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cjh.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lhp.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mkf.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://tnc.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jhj.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://edn.tarul.cn

[E22] 字节长度与字符长度
来源：http://rgx.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ojf.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugg.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tmm.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wir.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://neo.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aua.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://ato.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ees.shanyushiyangtech.top

================================================================================
来源：http://rdn.vqdsnc.cn

F. 文件与目录
来源：http://sbf.shzxlz.cn

================================================================================
来源：http://tav.chenjidiqi.icu

[F01] 读取整个文件
来源：http://mdf.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://snr.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://mqz.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nwr.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sny.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://spz.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xwd.smart0.xyz

Ruby: File.read("a.txt")
来源：http://rvl.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://bba.hnqzz.top

[F02] 逐行读取文件
来源：http://qle.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ayc.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iur.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://str.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bsb.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iau.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rpp.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gik.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://viz.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://vsv.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pcx.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://pxl.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyj.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://awg.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdb.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tlq.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://fnr.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vnx.yj20258888.top

[F04] 追加写入文件
来源：http://vly.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gcb.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://thl.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwu.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kav.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xvb.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mrd.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pfb.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hap.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://xrj.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yac.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://bul.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://kji.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://xnt.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pmb.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cip.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://qav.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://mrm.chenjidiqi.icu

[F06] 删除文件
来源：http://esd.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://ktr.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://upw.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ikv.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://alt.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://veh.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://cji.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://ckq.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://tfn.andypj.xyz

[F07] 创建目录（含多级）
来源：http://rss.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bvk.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dhv.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mnh.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgz.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yip.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zgf.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jte.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xmu.pengpengdd.cyou

[F08] 遍历目录
来源：http://lsk.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://awa.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ewq.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://vdm.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://lbi.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://adh.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jtc.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://qjw.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://sba.jiagoushi.top

[F09] 获取文件大小
来源：http://jtf.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://yzk.iojbl.cn

PHP:  filesize("a.txt");
来源：http://app.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://owm.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://aks.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wxa.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gwe.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://wui.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://jaz.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://asm.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jdw.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jox.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://osm.fktsv.cn

TS:   path.extname("a.txt")
来源：http://znp.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lvt.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dtg.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ncm.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jbp.yj202588.top

[F11] 复制与移动文件
来源：http://kbg.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pvt.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ros.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qob.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgo.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://agn.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ona.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qps.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jds.yj20258.top

[F12] CSV 读写
来源：http://fsy.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lyp.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lrl.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cbf.yanxiufei.cn

TS:   // 同上
来源：http://yyt.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://smu.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tth.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bwp.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kef.cdnleiting.top

================================================================================
来源：http://cfm.fengsongda.top

G. 面向对象
来源：http://hhf.zdqjudy.top

================================================================================
来源：http://wca.yfazqb.com

[G01] 定义类
来源：http://sjb.andypj.xyz

Py:   class User: pass
来源：http://orn.zdqjudy.top

PHP:  class User {}
来源：http://dbp.wangshuangyany.cn

JS:   class User {}
来源：http://rzd.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://sxt.gaohongyu789.top

Java: class User {}
来源：http://lhh.fktsv.cn

Go:   type User struct { Name string }
来源：http://pap.jinqigfzy.top

Ruby: class User; end
来源：http://wdy.yj20258888.top

C#:   class User {}
来源：http://zly.yvedp.cn

[G02] 构造函数
来源：http://cns.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://pfz.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://xrt.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://iuk.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://mik.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://vho.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iun.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://gfv.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://hbg.tanke756.top

[G03] 实例属性
来源：http://mds.zdbjq.cn

Py:   self.name = "x"
来源：http://xuw.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://eqq.yueranfly.top

JS:   this.name = "x";
来源：http://txj.shuidangran.top

TS:   name: string = "x";
来源：http://ltl.chenjidiqi.icu

Java: private String name;
来源：http://tdw.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sgv.zdbjq.cn

Ruby: @name = "x"
来源：http://uwh.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://uej.zhiwuduotai.top

[G04] 定义方法
来源：http://rlw.smart0.xyz

Py:   def greet(self): return self.name
来源：http://hdd.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jcw.hnqzz.top

JS:   greet() { return this.name; }
来源：http://row.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://uwa.nanxinkj.top

Java: String greet() { return name; }
来源：http://oqf.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jdd.aizwys.cn

Ruby: def greet; @name; end
来源：http://exw.fehbvm.com

C#:   public string Greet() => Name;
来源：http://wtf.nanxuanxn.top

[G05] 继承
来源：http://nvz.nanxinkj.top

Py:   class Admin(User): pass
来源：http://oad.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://anf.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://hfe.chenlongwang.top

TS:   class Admin extends User {}
来源：http://vae.daxiang520.top

Java: class Admin extends User {}
来源：http://tzx.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://utn.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://bem.ivvv.top

C#:   class Admin : User {}
来源：http://dgo.smart0.xyz

[G06] 重写方法
来源：http://mis.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://hov.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uaj.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://xgs.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://usb.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://frs.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://afw.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://ekm.vqdsnc.cn

C#:   public override string Greet() => "admin";
来源：http://vfa.nwbrower.top

[G07] 调用父类方法
来源：http://xwn.hysaishi.cn

Py:   super().greet()
来源：http://fpg.shangyingyoupin.top

PHP:  parent::greet();
来源：http://bpx.fktsv.cn

JS:   super.greet();
来源：http://uqz.jiagoushi.top

TS:   super.greet();
来源：http://ifg.hnqzz.top

Java: super.greet();
来源：http://msu.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lbi.guannengcc.top

Ruby: super
来源：http://cyi.52xcode.cn

C#:   base.Greet();
来源：http://qxa.52xcode.cn

[G08] 静态方法与属性
来源：http://ubi.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wgr.chenlongwang.top

PHP:  public static function f() {}
来源：http://qjg.fengsongda.top

JS:   static f() {}
来源：http://cdh.bjfxy.top

TS:   static f(): void {}
来源：http://pnt.aizwys.cn

Java: static void f() {}
来源：http://jsp.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rzr.jinqigufen.top

Ruby: def self.f; end
来源：http://kax.sweek.top

C#:   public static void F() {}
来源：http://fzo.ivvv.top

[G09] 接口 / 抽象类
来源：http://gbz.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://tsg.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://uck.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gzq.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://pat.fehbvm.com

Java: interface Shape { double area(); }
来源：http://tit.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://wyv.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nei.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://nvt.yanxiufei.cn

[G10] 访问控制
来源：http://fod.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://bho.bjfxy.top

PHP:  public / protected / private
来源：http://kom.ivvv.top

JS:   #private 字段；其余公开
来源：http://vlt.yongpay.top

TS:   public / protected / private
来源：http://cfr.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://fvo.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pxs.jyoumei.cn

Ruby: public / protected / private
来源：http://jig.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://gxc.ppjwa.cn

[G11] getter / setter
来源：http://ryq.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://qhe.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://oyp.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://xdv.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://myr.sweek.top

Java: public String getName() { return name; }
来源：http://cuk.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tnd.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://qrn.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://fsn.xylfe.cn

[G12] 对象转字符串
来源：http://cow.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://yuw.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://chk.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://tet.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://gjs.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://qbn.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://znl.gzhubu.top

Ruby: def to_s; @name; end
来源：http://xla.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://qpe.vqdsnc.cn

[G13] 判断对象类型
来源：http://hzj.xylfe.cn

Py:   isinstance(u, User)
来源：http://uwu.vehdjk.com

PHP:  $u instanceof User
来源：http://sow.zdqjudy.top

JS:   u instanceof User
来源：http://hgs.hammf.cn

TS:   u instanceof User
来源：http://vcj.yvedp.cn

Java: u instanceof User
来源：http://bjy.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xyj.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://tnh.daxiang520.top

C#:   u is User
来源：http://ftr.jqgfzy.top

[G14] 数据类 / record
来源：http://mas.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fyn.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://bev.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xwz.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://inv.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://mjn.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://clp.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dqd.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://ove.hywenlv.cn

[G15] 枚举
来源：http://ief.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bmz.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wvs.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dfi.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npl.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://ikg.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zsl.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://lkr.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://axy.cashguo.top

[G16] 对象转数组 / 字典
来源：http://maw.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wkb.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://rck.redwolf501.top

JS:   Object.entries(obj)
来源：http://ltp.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://swp.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bcr.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rxr.cdnleiting.top

Ruby: obj.instance_variables
来源：http://ntz.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://zra.jyoumei.cn

================================================================================
来源：http://zsa.haohaochexian.top

H. 异常与错误处理
来源：http://ezp.jyoumei.cn

================================================================================
来源：http://xsj.chenzaomai.com

[H01] try / catch 基础
来源：http://ruw.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://med.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ssc.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nns.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qhz.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sdg.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gll.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sgo.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dbb.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://ejf.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gcc.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://plc.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qyh.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cyg.kuanghao11.cn


<!-- 参考信息 -->