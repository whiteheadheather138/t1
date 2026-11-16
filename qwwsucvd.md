代发 wailian999

Ruby: s.lines
来源：http://mhd.zdqjudy.top

C#:   s.Split('\n')
来源：http://ats.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://nnd.fehbvm.com

Py:   if not s:
来源：http://ryo.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rou.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://els.bbcook.cn

TS:   if (s === "") {}
来源：http://dtq.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://fbe.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://suy.dashuyun.cn

Ruby: if s.empty?
来源：http://pai.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jav.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://gjv.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hpn.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kko.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rts.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sfe.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pis.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://fxd.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wfs.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnu.mhx1999.top

[E22] 字节长度与字符长度
来源：http://wwu.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vjf.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zxn.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yoi.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wlr.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dls.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vwg.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://quo.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yqr.yj20258888.top

================================================================================
来源：http://pbf.hnxiangtu.top

F. 文件与目录
来源：http://xbi.smart0.xyz

================================================================================
来源：http://onf.meibo888.top

[F01] 读取整个文件
来源：http://gze.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hqo.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://xpm.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hsp.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://del.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oqv.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ypp.daria6918.cn

Ruby: File.read("a.txt")
来源：http://wyw.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://nrw.fktsv.cn

[F02] 逐行读取文件
来源：http://rrw.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rke.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lzk.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tlt.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpv.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://igt.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ovh.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vme.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://brf.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://req.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lep.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xlb.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dny.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkb.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://agv.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gfq.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://szk.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uso.redwolf501.top

[F04] 追加写入文件
来源：http://ekw.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://thx.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ggy.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ayf.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijd.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lvn.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lqh.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ahs.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pqk.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://vfm.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lpu.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://kxc.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://pou.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://dge.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qwq.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iik.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://gqm.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://ovz.guannengcc.top

[F06] 删除文件
来源：http://xrf.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://sgm.fktsv.cn

PHP:  unlink("a.txt");
来源：http://vkt.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hhu.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://tzb.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qog.uphjek.com

Go:   os.Remove("a.txt")
来源：http://tci.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://imk.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://vbp.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://sjv.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aap.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mco.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://atm.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ykw.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xld.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sti.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lid.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://utk.hesvh.cn

[F08] 遍历目录
来源：http://gzv.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://txx.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zlc.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://adu.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://xwt.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eio.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hca.bjfxy.top

Ruby: Dir.children("dir")
来源：http://jjv.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://rfu.snrcjt.cn

[F09] 获取文件大小
来源：http://wcf.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://nda.bbcook.cn

PHP:  filesize("a.txt");
来源：http://dtg.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://pyo.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://jyx.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oee.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xwa.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://ucp.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://mub.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://obr.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mnx.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yze.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://max.redwolf501.top

TS:   path.extname("a.txt")
来源：http://qdv.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sja.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pby.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bbe.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fqy.jianghu66.top

[F11] 复制与移动文件
来源：http://jil.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://efb.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zhz.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ogt.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fox.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://img.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://avt.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://umh.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://faj.zdqjudy.top

[F12] CSV 读写
来源：http://ibi.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cve.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mul.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tit.shzxlz.cn

TS:   // 同上
来源：http://xgm.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mmr.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jrn.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hue.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://hkl.tianlin.xyz

================================================================================
来源：http://rav.ydzc1.top

G. 面向对象
来源：http://vkl.nanxuanxn.top

================================================================================
来源：http://ueo.zhixingplan.top

[G01] 定义类
来源：http://xjh.hywenlv.cn

Py:   class User: pass
来源：http://nri.hnqzz.top

PHP:  class User {}
来源：http://hpt.cashguo.top

JS:   class User {}
来源：http://nki.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://vdg.vqdsnc.cn

Java: class User {}
来源：http://yzo.hfpthk.cn

Go:   type User struct { Name string }
来源：http://wdu.svipenyu.cn

Ruby: class User; end
来源：http://wkf.xziqi.cn

C#:   class User {}
来源：http://fce.shangyingyoupin.top

[G02] 构造函数
来源：http://qpb.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://jsn.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://mtj.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://btt.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://ggo.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://tgw.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pkp.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://fil.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://cgu.fanxiaobao.xyz

[G03] 实例属性
来源：http://vle.yj20258888.top

Py:   self.name = "x"
来源：http://pjs.hammf.cn

PHP:  public string $name = "x";
来源：http://oou.shuidangran.top

JS:   this.name = "x";
来源：http://bqj.fengsongda.top

TS:   name: string = "x";
来源：http://dyr.shzxlz.cn

Java: private String name;
来源：http://iqr.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mfc.gzhubu.top

Ruby: @name = "x"
来源：http://qyu.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://vzh.yueranfly.top

[G04] 定义方法
来源：http://zyn.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://udw.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kep.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://mfa.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://qje.hysaishi.cn

Java: String greet() { return name; }
来源：http://osf.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jnc.svipenyu.cn

Ruby: def greet; @name; end
来源：http://xgj.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://jst.mhx1999.top

[G05] 继承
来源：http://qvj.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://bco.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://qzo.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://vcb.yfazqb.com

TS:   class Admin extends User {}
来源：http://exu.zhixingplan.top

Java: class Admin extends User {}
来源：http://gou.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nkw.zhengqikj.top

Ruby: class Admin < User; end
来源：http://sso.tarul.cn

C#:   class Admin : User {}
来源：http://wlr.hywenlv.cn

[G06] 重写方法
来源：http://cnf.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://tdd.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rfo.meibo888.top

JS:   greet() { return "admin"; }
来源：http://kga.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://izq.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://bal.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://woy.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://htv.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://rtv.jlsjyb.cn

[G07] 调用父类方法
来源：http://oab.yueranfly.top

Py:   super().greet()
来源：http://eop.ppjwa.cn

PHP:  parent::greet();
来源：http://isl.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://bia.hnqzz.top

TS:   super.greet();
来源：http://qzj.ppjwa.cn

Java: super.greet();
来源：http://dmj.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nem.sweek.top

Ruby: super
来源：http://gph.xinyue.icu

C#:   base.Greet();
来源：http://tgz.daxiang520.top

[G08] 静态方法与属性
来源：http://gek.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iyg.zycfv.cn

PHP:  public static function f() {}
来源：http://lut.hfpthk.cn

JS:   static f() {}
来源：http://bbr.havefunace.top

TS:   static f(): void {}
来源：http://ire.uphjek.com

Java: static void f() {}
来源：http://rfy.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oww.cashguo.top

Ruby: def self.f; end
来源：http://wia.wangdashe.top

C#:   public static void F() {}
来源：http://tad.sweek.top

[G09] 接口 / 抽象类
来源：http://eub.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://fwu.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://afj.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://hox.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://agy.yuxming.cn

Java: interface Shape { double area(); }
来源：http://rim.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://fmv.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nxi.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://ext.gzhubu.top

[G10] 访问控制
来源：http://soq.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://vsj.hongshengwenyu.top

PHP:  public / protected / private
来源：http://xty.redwolf501.top

JS:   #private 字段；其余公开
来源：http://rvo.c1oappe.top

TS:   public / protected / private
来源：http://pid.havefunace.top

Java: public / protected / private / 默认包级
来源：http://qyl.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://gxm.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://gah.hywenlv.cn

C#:   public / protected / private / internal
来源：http://csr.tian-w.cn

[G11] getter / setter
来源：http://wot.sxryk.cn

Py:   @property 与 @x.setter
来源：http://rmj.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qku.yueranfly.top

JS:   get name() { return this._name; }
来源：http://yck.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://oon.andypj.xyz

Java: public String getName() { return name; }
来源：http://enp.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cct.hesvh.cn

Ruby: attr_accessor :name
来源：http://hyl.daxiang520.top

C#:   public string Name { get; set; }
来源：http://ajb.yonumen.top

[G12] 对象转字符串
来源：http://zvh.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://khy.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tme.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://ipo.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://fbh.chenzaomai.com

Java: @Override public String toString() { return name; }
来源：http://zmb.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://dbf.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://sar.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://wmq.bbcook.cn

[G13] 判断对象类型
来源：http://aoo.vehdjk.com

Py:   isinstance(u, User)
来源：http://via.nanxinkj.top

PHP:  $u instanceof User
来源：http://gjy.zhoulong.xyz

JS:   u instanceof User
来源：http://eeh.shangyingyoupin.top

TS:   u instanceof User
来源：http://yzg.zhengqikj.top

Java: u instanceof User
来源：http://lvs.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://dfe.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://lci.9152youxi.cn

C#:   u is User
来源：http://tcz.yvedp.cn

[G14] 数据类 / record
来源：http://unz.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gzs.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://qtl.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://epz.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://sux.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://ntp.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://lui.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://knm.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://meb.yuanzhike.top

[G15] 枚举
来源：http://kmp.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://chf.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oko.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qli.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fpq.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://xix.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dkp.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://ocs.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://urp.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://xvu.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tvn.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://wrj.iojbl.cn

JS:   Object.entries(obj)
来源：http://jzt.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://aat.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://prq.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rlk.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://mpl.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://hpq.quarkkingdee.top

================================================================================
来源：http://qpy.yueranfly.top

H. 异常与错误处理
来源：http://spo.yj20258.top

================================================================================
来源：http://xod.zhoulong.xyz

[H01] try / catch 基础
来源：http://lkr.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dlx.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qgx.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hhw.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xfj.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gel.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lhu.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qcn.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xki.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://jdo.smart0.xyz


<!-- 参考信息 -->