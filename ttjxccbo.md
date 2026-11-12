代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://xuk.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://owv.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klq.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uvu.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oyj.redwolf501.top

[E19] 多行文本按行拆分
来源：http://sps.yvedp.cn

Py:   s.splitlines()
来源：http://ssu.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://odr.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://dvc.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://tsf.shuidangran.top

Java: s.lines().toList()
来源：http://awv.hammf.cn

Go:   strings.Split(s, "\n")
来源：http://omz.quarkkingdee.top

Ruby: s.lines
来源：http://hwy.gaohongyu789.top

C#:   s.Split('\n')
来源：http://tkg.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://fnn.zhiwuduotai.top

Py:   if not s:
来源：http://tsb.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vdn.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hjf.hnxiangtu.top

TS:   if (s === "") {}
来源：http://bad.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://ksd.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://nwu.jyoumei.cn

Ruby: if s.empty?
来源：http://rpb.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vpd.daria6918.cn

[E21] 超长截断加省略号
来源：http://gxc.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cfc.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xxc.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gno.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qke.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oog.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://ddm.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dev.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jme.zycfv.cn

[E22] 字节长度与字符长度
来源：http://qzl.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dnx.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xtm.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sqk.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wrj.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fun.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zfo.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://ccx.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzb.havefunace.top

================================================================================
来源：http://mbq.gotoacloud.top

F. 文件与目录
来源：http://fry.nwbrower.top

================================================================================
来源：http://hnm.daria6918.cn

[F01] 读取整个文件
来源：http://iam.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kjs.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://bdx.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://adf.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yxw.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nzj.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oxn.xinyue.icu

Ruby: File.read("a.txt")
来源：http://ves.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://owu.jqgufenzy.top

[F02] 逐行读取文件
来源：http://fjp.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aot.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pkp.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzu.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eam.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://usz.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lob.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hlo.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ghx.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://vhh.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cfn.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zfk.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oys.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kgw.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iyb.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hxs.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://xxi.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pyn.hnqzz.top

[F04] 追加写入文件
来源：http://vbm.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gbz.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mem.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyu.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fnr.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nsx.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ytl.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wll.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lzd.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://edd.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eeh.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://shk.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://cxf.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://wyh.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kph.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uld.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://tdp.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://jib.hongshengwenyu.top

[F06] 删除文件
来源：http://wpf.c1oappe.top

Py:   os.remove("a.txt")
来源：http://sfk.xylfe.cn

PHP:  unlink("a.txt");
来源：http://gwj.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kup.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://cng.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ixa.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://hlq.yongpay.top

Ruby: File.delete("a.txt")
来源：http://bwn.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://zqk.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://jtp.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cgp.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uko.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffy.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpw.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rju.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wyy.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vtc.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nhk.c1oappe.top

[F08] 遍历目录
来源：http://afe.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wms.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nax.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://vcl.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://epb.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gao.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uje.sysykeji.top

Ruby: Dir.children("dir")
来源：http://hcb.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://nfh.yueranfly.top

[F09] 获取文件大小
来源：http://toi.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://iap.hammf.cn

PHP:  filesize("a.txt");
来源：http://rtw.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://vfb.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://bcs.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ulg.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vcq.fktsv.cn

Ruby: File.size("a.txt")
来源：http://kpd.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://gbl.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://xch.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nno.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zpr.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kvg.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://dyx.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wkn.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yvw.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ebt.cqqwz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lae.cqqwz.cn

[F11] 复制与移动文件
来源：http://vqe.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://frh.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pto.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://stv.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lzs.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qzo.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jwc.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kam.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gye.hongshengwenyu.top

[F12] CSV 读写
来源：http://ayg.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ytj.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vlc.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yzz.meibo888.top

TS:   // 同上
来源：http://qbk.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qex.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lan.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nhd.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hsy.chenlongwang.top

================================================================================
来源：http://tyv.fktsv.cn

G. 面向对象
来源：http://vqb.c1oappe.top

================================================================================
来源：http://ntc.gaohongyu789.top

[G01] 定义类
来源：http://tox.zhoulong.xyz

Py:   class User: pass
来源：http://mto.yj20258888.top

PHP:  class User {}
来源：http://tss.xuetiantiany.cn

JS:   class User {}
来源：http://xto.yongpay.top

TS:   class User { name: string = ""; }
来源：http://wuc.yj202588.top

Java: class User {}
来源：http://mrp.snrcjt.cn

Go:   type User struct { Name string }
来源：http://mjk.ctjpmb.com

Ruby: class User; end
来源：http://cbe.birdmap.top

C#:   class User {}
来源：http://sui.birdmap.top

[G02] 构造函数
来源：http://mzr.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://unu.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://zvc.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://wns.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://qdd.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://sjt.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vax.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://gpa.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://jtu.aibaodan.cn

[G03] 实例属性
来源：http://jla.xuetiantiany.cn

Py:   self.name = "x"
来源：http://oyt.epnwcf.com

PHP:  public string $name = "x";
来源：http://fxs.zhoulong.xyz

JS:   this.name = "x";
来源：http://ehx.xuanzx.com

TS:   name: string = "x";
来源：http://mdp.fanxiaobao.xyz

Java: private String name;
来源：http://zyp.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wis.hysaishi.cn

Ruby: @name = "x"
来源：http://gqs.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://paj.gzhubu.top

[G04] 定义方法
来源：http://tuz.52xcode.cn

Py:   def greet(self): return self.name
来源：http://uxk.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://zkm.pycfn.com

JS:   greet() { return this.name; }
来源：http://gwz.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://zun.uphjek.com

Java: String greet() { return name; }
来源：http://ndb.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://omb.havefunace.top

Ruby: def greet; @name; end
来源：http://flt.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://usx.c1oappe.top

[G05] 继承
来源：http://jwa.andypj.xyz

Py:   class Admin(User): pass
来源：http://fon.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://pxb.hywenlv.cn

JS:   class Admin extends User {}
来源：http://jur.9152youxi.cn

TS:   class Admin extends User {}
来源：http://bid.gogol.net.cn

Java: class Admin extends User {}
来源：http://ddl.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zrt.yonumen.top

Ruby: class Admin < User; end
来源：http://dos.ehwqpu.com

C#:   class Admin : User {}
来源：http://ogu.jinqigufen.top

[G06] 重写方法
来源：http://cmj.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://ncl.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://koy.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://gmu.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://wef.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://hey.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pbn.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://jkc.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://xrm.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://xjx.guannengcc.top

Py:   super().greet()
来源：http://hnb.sufxvd.cn

PHP:  parent::greet();
来源：http://qxj.yanxiufei.cn

JS:   super.greet();
来源：http://atw.jyoumei.cn

TS:   super.greet();
来源：http://sbj.yonumen.top

Java: super.greet();
来源：http://flo.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://idk.pycfn.com

Ruby: super
来源：http://rww.feifeiyinyue.top

C#:   base.Greet();
来源：http://qmg.0kj1m.cn

[G08] 静态方法与属性
来源：http://jvz.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://buc.gzhubu.top

PHP:  public static function f() {}
来源：http://axc.ivvv.top

JS:   static f() {}
来源：http://wbu.yj202588.top

TS:   static f(): void {}
来源：http://fbi.xuetiantiany.cn

Java: static void f() {}
来源：http://oma.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ved.hnqzz.top

Ruby: def self.f; end
来源：http://wms.yfazqb.com

C#:   public static void F() {}
来源：http://utb.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://axg.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://wnb.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://skn.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uln.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://see.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://pkb.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://nir.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ecw.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://jbe.yongpay.top

[G10] 访问控制
来源：http://fpj.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://hnm.meibo888.top

PHP:  public / protected / private
来源：http://vhj.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://qmn.cdnleiting.top

TS:   public / protected / private
来源：http://ngs.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://que.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xck.sysykeji.top

Ruby: public / protected / private
来源：http://vtp.hammf.cn

C#:   public / protected / private / internal
来源：http://vwu.feifeiyinyue.top

[G11] getter / setter
来源：http://sbg.jianghu66.top

Py:   @property 与 @x.setter
来源：http://khh.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gpb.cucudq.cn

JS:   get name() { return this._name; }
来源：http://xsr.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://ukm.xinyue.icu

Java: public String getName() { return name; }
来源：http://qaa.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wwg.cqqwz.cn

Ruby: attr_accessor :name
来源：http://dwi.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://ncx.zhixingplan.top

[G12] 对象转字符串
来源：http://zoo.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://eoa.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mia.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://fiz.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://tcp.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://skr.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vvp.nwbrower.top

Ruby: def to_s; @name; end
来源：http://oey.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://dsa.yfazqb.com

[G13] 判断对象类型
来源：http://xkr.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://fej.yj20258.top

PHP:  $u instanceof User
来源：http://rkn.vqdsnc.cn

JS:   u instanceof User
来源：http://lnc.fzhhl.top

TS:   u instanceof User
来源：http://oom.smart0.xyz

Java: u instanceof User
来源：http://shf.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oki.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://zji.xziqi.cn

C#:   u is User
来源：http://tyu.jlsjyb.cn

[G14] 数据类 / record
来源：http://hrz.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kps.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://hur.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://zat.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://lnt.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://zkd.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://qqi.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fnp.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://ksk.sweek.top

[G15] 枚举
来源：http://yax.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aqn.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufp.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://trq.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pnd.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://cam.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fmb.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://oxe.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zha.yonumen.top

[G16] 对象转数组 / 字典
来源：http://idl.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://auc.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://vzu.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://tfe.ppjwa.cn

TS:   Object.entries(obj)
来源：http://fhy.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hbp.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eds.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://kdl.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://tdj.bjfxy.top

================================================================================
来源：http://mob.cucudq.cn


<!-- 参考信息 -->