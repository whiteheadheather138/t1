代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://fyb.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xfd.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xcp.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://akh.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://szv.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://ewu.aibaodan.cn

Py:   s.splitlines()
来源：http://mwh.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://trt.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://dpv.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://aiw.yueranfly.top

Java: s.lines().toList()
来源：http://itp.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://cwg.xuetiantiany.cn

Ruby: s.lines
来源：http://mwh.vqdsnc.cn

C#:   s.Split('\n')
来源：http://xkt.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://ezg.tanke756.top

Py:   if not s:
来源：http://jqm.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hlu.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmw.hysaishi.cn

TS:   if (s === "") {}
来源：http://stx.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://tge.smart0.xyz

Go:   if s == "" {}
来源：http://xsq.yj202588.top

Ruby: if s.empty?
来源：http://xay.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mes.sysykeji.top

[E21] 超长截断加省略号
来源：http://fcs.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qex.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpl.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lal.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mtg.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cav.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://juz.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ipc.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dqv.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://lhp.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nol.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzw.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cds.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zvi.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qrd.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oxh.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://uzb.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wjz.daria6918.cn

================================================================================
来源：http://ehc.dianchejie.cn

F. 文件与目录
来源：http://ior.shzxlz.cn

================================================================================
来源：http://tgp.316326.xyz

[F01] 读取整个文件
来源：http://vly.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mdx.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://xib.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ybt.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mkh.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rjn.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iiv.tarul.cn

Ruby: File.read("a.txt")
来源：http://zmv.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://eyp.aizwys.cn

[F02] 逐行读取文件
来源：http://jiy.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eew.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xeq.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awi.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sqa.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cit.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jbf.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qdi.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tvo.yonumen.top

[F03] 写入文件（覆盖）
来源：http://ftt.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://swi.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rhi.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jql.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrp.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lkx.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ahr.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://vjv.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pqr.xuetiantiany.cn

[F04] 追加写入文件
来源：http://vpq.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xzd.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kdk.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwf.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jef.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://biu.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ete.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bkl.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dfj.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://qwm.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bfr.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://kue.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://dhd.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://wds.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jrx.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vwl.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://lyw.birdmap.top

C#:   File.Exists("a.txt")
来源：http://axx.dashuyun.cn

[F06] 删除文件
来源：http://rvv.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://qru.ybcxt.top

PHP:  unlink("a.txt");
来源：http://lxq.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://ssr.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://fca.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mro.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://mkp.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://czy.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://yni.c1oappe.top

[F07] 创建目录（含多级）
来源：http://mmf.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jje.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aae.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://buf.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sdr.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fyr.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rxn.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvg.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ijl.tanke756.top

[F08] 遍历目录
来源：http://mby.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://crr.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zch.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://fip.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://vnn.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kdj.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rfg.c1oappe.top

Ruby: Dir.children("dir")
来源：http://kmi.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://gxh.vqdsnc.cn

[F09] 获取文件大小
来源：http://tsx.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://vlv.sweek.top

PHP:  filesize("a.txt");
来源：http://vzk.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://etd.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://pfx.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gdi.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qcq.ydzc1.top

Ruby: File.size("a.txt")
来源：http://srp.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://qfb.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://ukt.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wjl.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tkz.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cqr.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://lhm.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://huy.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pkl.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://avm.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjh.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://dfl.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vrd.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xzt.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nuj.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qqa.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yod.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vkl.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zyk.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pjd.ehwqpu.com

[F12] CSV 读写
来源：http://rjl.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://agd.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hck.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rfq.zhiwuduotai.top

TS:   // 同上
来源：http://hpw.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kil.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yhu.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vox.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wgz.smart0.xyz

================================================================================
来源：http://loq.jqgfzy.top

G. 面向对象
来源：http://dph.jianghu66.top

================================================================================
来源：http://ste.jiagoushi.top

[G01] 定义类
来源：http://ker.shuidangran.top

Py:   class User: pass
来源：http://pyc.yj20258888.top

PHP:  class User {}
来源：http://gld.hnqzz.top

JS:   class User {}
来源：http://rtf.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://vzc.jinyuanbaomall.cn

Java: class User {}
来源：http://eow.0kj1m.cn

Go:   type User struct { Name string }
来源：http://ypp.c1oappe.top

Ruby: class User; end
来源：http://ufi.smart0.xyz

C#:   class User {}
来源：http://yoh.redwolf501.top

[G02] 构造函数
来源：http://eey.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://axe.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://mbs.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://bti.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://jzp.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://ftx.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xko.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://wjt.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://svw.vehdjk.com

[G03] 实例属性
来源：http://nya.chenzaomai.com

Py:   self.name = "x"
来源：http://hyl.zycfv.cn

PHP:  public string $name = "x";
来源：http://fxq.zdbjq.cn

JS:   this.name = "x";
来源：http://cjr.cucudq.cn

TS:   name: string = "x";
来源：http://iea.jinqigfzy.top

Java: private String name;
来源：http://luu.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qkm.xziqi.cn

Ruby: @name = "x"
来源：http://yzh.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://koq.yanxiufei.cn

[G04] 定义方法
来源：http://cae.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://qjm.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vks.c1oappe.top

JS:   greet() { return this.name; }
来源：http://aae.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://oho.ctjpmb.com

Java: String greet() { return name; }
来源：http://ior.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://klh.nanxinkj.top

Ruby: def greet; @name; end
来源：http://hlb.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://nqd.fanxiaobao.xyz

[G05] 继承
来源：http://ipj.epnwcf.com

Py:   class Admin(User): pass
来源：http://qpd.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://prr.zdqjudy.top

JS:   class Admin extends User {}
来源：http://bvr.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://lwl.shuidangran.top

Java: class Admin extends User {}
来源：http://ryg.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eto.dianchejie.cn

Ruby: class Admin < User; end
来源：http://tss.fktsv.cn

C#:   class Admin : User {}
来源：http://zhq.xinyue.icu

[G06] 重写方法
来源：http://qfs.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://tho.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qrw.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://vcm.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://wqk.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://lqg.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cqm.hammf.cn

Ruby: def greet; "admin"; end
来源：http://orh.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://qdi.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://nhb.kuanghao11.cn

Py:   super().greet()
来源：http://eqb.andypj.xyz

PHP:  parent::greet();
来源：http://cgx.guowangkeji.top

JS:   super.greet();
来源：http://twb.fanxiaobao.xyz

TS:   super.greet();
来源：http://qzs.uphjek.com

Java: super.greet();
来源：http://pzf.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kce.epnwcf.com

Ruby: super
来源：http://hed.fengsongda.top

C#:   base.Greet();
来源：http://fks.redwolf501.top

[G08] 静态方法与属性
来源：http://gux.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://swu.wangdashe.top

PHP:  public static function f() {}
来源：http://osj.gotoacloud.top

JS:   static f() {}
来源：http://cml.xinyue.icu

TS:   static f(): void {}
来源：http://eup.sufxvd.cn

Java: static void f() {}
来源：http://qtq.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xyx.jianghu66.top

Ruby: def self.f; end
来源：http://uqz.hysaishi.cn

C#:   public static void F() {}
来源：http://bbu.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://qrw.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://apv.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://jnj.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qrn.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://ccd.fktsv.cn

Java: interface Shape { double area(); }
来源：http://zkx.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://sbk.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xix.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://wyi.sjlbkw.cn

[G10] 访问控制
来源：http://grx.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://bzp.ybcxt.top

PHP:  public / protected / private
来源：http://ymo.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://ken.vqdsnc.cn

TS:   public / protected / private
来源：http://tlg.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://bqj.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zjm.yanxiufei.cn

Ruby: public / protected / private
来源：http://ffg.ctjpmb.com

C#:   public / protected / private / internal
来源：http://gyp.snrcjt.cn

[G11] getter / setter
来源：http://pwr.nwbrower.top

Py:   @property 与 @x.setter
来源：http://urr.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bom.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://fmz.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://oxp.hcnkem.com

Java: public String getName() { return name; }
来源：http://duz.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sjp.cqqwz.cn

Ruby: attr_accessor :name
来源：http://sxf.sysykeji.top

C#:   public string Name { get; set; }
来源：http://ova.yj20258888.top

[G12] 对象转字符串
来源：http://kwl.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://mro.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rdq.havefunace.top

JS:   toString() { return this.name; }
来源：http://nmv.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://ybn.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://wco.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://jrh.cucudq.cn

Ruby: def to_s; @name; end
来源：http://wya.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://bap.hcnkem.com

[G13] 判断对象类型
来源：http://drk.chenzaomai.com

Py:   isinstance(u, User)
来源：http://qky.xuanzx.com

PHP:  $u instanceof User
来源：http://tkn.fanxiaobao.xyz

JS:   u instanceof User
来源：http://hmy.zdbjq.cn

TS:   u instanceof User
来源：http://kzn.xziqi.cn

Java: u instanceof User
来源：http://hpc.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ucc.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://dvz.havefunace.top

C#:   u is User
来源：http://lqw.hnxiangtu.top

[G14] 数据类 / record
来源：http://xdt.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jhc.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://fvv.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://chz.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://umv.daria6918.cn

Java: record User(String name, int age) {}
来源：http://xiw.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://qtb.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ywe.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://nfh.yonumen.top

[G15] 枚举
来源：http://ugo.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://opr.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bvt.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kmm.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kbi.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://nqo.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://apb.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://jgw.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tel.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://qqz.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xfh.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://uqd.iojbl.cn

JS:   Object.entries(obj)
来源：http://snw.cqqwz.cn

TS:   Object.entries(obj)
来源：http://oka.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zpa.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://axs.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://dyc.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://bli.haohaochexian.top

================================================================================
来源：http://aim.sxryk.cn


<!-- 参考信息 -->