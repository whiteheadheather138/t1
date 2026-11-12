代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xbp.xylfe.cn

[E19] 多行文本按行拆分
来源：http://fgp.birdmap.top

Py:   s.splitlines()
来源：http://iun.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vwn.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://mrv.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://fve.xziqi.cn

Java: s.lines().toList()
来源：http://ayz.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://gtn.0kj1m.cn

Ruby: s.lines
来源：http://ypt.tianlin.xyz

C#:   s.Split('\n')
来源：http://jlx.daria6918.cn

[E20] 判断字符串是否为空
来源：http://zvp.xuanzx.com

Py:   if not s:
来源：http://yqe.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mhp.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://htj.hammf.cn

TS:   if (s === "") {}
来源：http://ksj.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://wns.cdnleiting.top

Go:   if s == "" {}
来源：http://orv.sufxvd.cn

Ruby: if s.empty?
来源：http://tab.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bcw.zdqjudy.top

[E21] 超长截断加省略号
来源：http://olp.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xnc.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tuu.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ddl.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cxw.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dwd.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://hjn.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://trj.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aaz.cashguo.top

[E22] 字节长度与字符长度
来源：http://hft.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mta.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gul.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kkh.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dxx.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nma.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uko.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://nye.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://htm.snrcjt.cn

================================================================================
来源：http://xxu.jianghu66.top

F. 文件与目录
来源：http://dqr.zdqjudy.top

================================================================================
来源：http://def.yvedp.cn

[F01] 读取整个文件
来源：http://sxq.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fet.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://dij.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://css.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzi.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kde.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hqv.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://syp.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://srl.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://slc.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://glc.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hsr.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bhv.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vmc.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://krv.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mxi.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qhe.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjg.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://mzl.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gjx.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ozu.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nix.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://htr.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ovg.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gxl.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://zgh.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nur.jyoumei.cn

[F04] 追加写入文件
来源：http://hub.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fcb.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lve.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxz.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qgo.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://exk.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uys.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://unp.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://chr.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://ilj.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ysj.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://kmb.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://qzp.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://cvy.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hiv.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gvu.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://uvm.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://qro.hnxiangtu.top

[F06] 删除文件
来源：http://ygc.pycfn.com

Py:   os.remove("a.txt")
来源：http://qvj.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://fih.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://sni.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fsg.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xuu.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://mxb.yj20258.top

Ruby: File.delete("a.txt")
来源：http://rae.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://rud.yongpay.top

[F07] 创建目录（含多级）
来源：http://oyg.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sga.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbs.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xbw.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ugh.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oyz.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyh.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nhk.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://glh.vqdsnc.cn

[F08] 遍历目录
来源：http://ghg.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mgc.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qzm.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://hfm.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://lpm.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ueu.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ktz.cashguo.top

Ruby: Dir.children("dir")
来源：http://nrx.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://iww.ybcxt.top

[F09] 获取文件大小
来源：http://zmv.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://srk.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://ufo.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://uko.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://jmy.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://zwi.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mos.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://bec.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://oan.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://vbv.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zad.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lgw.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ddb.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://xku.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dhb.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uon.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://idm.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mpn.pycfn.com

[F11] 复制与移动文件
来源：http://wiq.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fbg.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xyc.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://faw.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xas.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qes.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gcq.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://avy.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fvj.vqdsnc.cn

[F12] CSV 读写
来源：http://awa.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qrs.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ypm.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqi.tarul.cn

TS:   // 同上
来源：http://qhk.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://krr.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nlf.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aja.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wvr.fktsv.cn

================================================================================
来源：http://ilb.jinyuanbaomall.cn

G. 面向对象
来源：http://dtz.yueranfly.top

================================================================================
来源：http://oxb.tianlin.xyz

[G01] 定义类
来源：http://avj.yfazqb.com

Py:   class User: pass
来源：http://tig.daria6918.cn

PHP:  class User {}
来源：http://con.chenjidiqi.icu

JS:   class User {}
来源：http://jre.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://acu.kuanghao11.cn

Java: class User {}
来源：http://alk.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://nqx.bbcook.cn

Ruby: class User; end
来源：http://gbx.guowangkeji.top

C#:   class User {}
来源：http://dju.hnqzz.top

[G02] 构造函数
来源：http://kbx.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://zzz.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://mek.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://qjn.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://tda.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://yqr.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lqq.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://vys.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://dgs.dashuyun.cn

[G03] 实例属性
来源：http://irp.epnwcf.com

Py:   self.name = "x"
来源：http://hoh.zdbjq.cn

PHP:  public string $name = "x";
来源：http://cec.yanxiufei.cn

JS:   this.name = "x";
来源：http://ueq.zhengqikj.top

TS:   name: string = "x";
来源：http://ztx.zdbjq.cn

Java: private String name;
来源：http://txq.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tvw.andypj.xyz

Ruby: @name = "x"
来源：http://spa.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://bxf.cashguo.top

[G04] 定义方法
来源：http://tnx.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://xxh.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://opk.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://neq.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://cxa.bjfxy.top

Java: String greet() { return name; }
来源：http://xya.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pck.dianchejie.cn

Ruby: def greet; @name; end
来源：http://whd.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://lpv.fanxiaobao.xyz

[G05] 继承
来源：http://xjn.fktsv.cn

Py:   class Admin(User): pass
来源：http://cnu.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://dlr.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://wvw.fzhhl.top

TS:   class Admin extends User {}
来源：http://npq.dianchejie.cn

Java: class Admin extends User {}
来源：http://syi.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://guo.birdmap.top

Ruby: class Admin < User; end
来源：http://xwn.hcnkem.com

C#:   class Admin : User {}
来源：http://vho.yonumen.top

[G06] 重写方法
来源：http://csm.uphjek.com

Py:   def greet(self): return "admin"
来源：http://qjo.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://baa.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://iww.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://ecz.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://ezg.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tom.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://cns.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://ryb.yvedp.cn

[G07] 调用父类方法
来源：http://zyp.nanxinkj.top

Py:   super().greet()
来源：http://vya.guowangkeji.top

PHP:  parent::greet();
来源：http://dgm.zhengqikj.top

JS:   super.greet();
来源：http://ngi.zdqjudy.top

TS:   super.greet();
来源：http://qqd.xziqi.cn

Java: super.greet();
来源：http://eqq.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gih.gogol.net.cn

Ruby: super
来源：http://ehm.chenzaomai.com

C#:   base.Greet();
来源：http://snc.yanxiufei.cn

[G08] 静态方法与属性
来源：http://zdk.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://teb.tian-w.cn

PHP:  public static function f() {}
来源：http://qzu.ywan-chungtsiang.top

JS:   static f() {}
来源：http://vvp.cdnleiting.top

TS:   static f(): void {}
来源：http://ymk.fehbvm.com

Java: static void f() {}
来源：http://zly.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wjj.zhengqikj.top

Ruby: def self.f; end
来源：http://iwn.havefunace.top

C#:   public static void F() {}
来源：http://qat.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://nms.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://rqq.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dbi.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pul.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://prp.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://kox.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://zzb.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jdt.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://pqt.snrcjt.cn

[G10] 访问控制
来源：http://atz.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://hum.shzxlz.cn

PHP:  public / protected / private
来源：http://gaa.c1oappe.top

JS:   #private 字段；其余公开
来源：http://gkf.cheryme.top

TS:   public / protected / private
来源：http://kvg.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://yun.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oji.tanke756.top

Ruby: public / protected / private
来源：http://lsl.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://drv.yuanzhike.top

[G11] getter / setter
来源：http://jto.iojbl.cn

Py:   @property 与 @x.setter
来源：http://nnf.ydjk.org.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rpu.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://rjc.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://bve.havefunace.top

Java: public String getName() { return name; }
来源：http://tdf.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zlw.svipenyu.cn

Ruby: attr_accessor :name
来源：http://lvc.redwolf501.top

C#:   public string Name { get; set; }
来源：http://xgn.chenlongwang.top

[G12] 对象转字符串
来源：http://cpc.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://xam.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://hjp.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://wop.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://hsi.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://xxy.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://idi.aizwys.cn

Ruby: def to_s; @name; end
来源：http://ngz.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://kuj.yj202588.top

[G13] 判断对象类型
来源：http://htl.meibo888.top

Py:   isinstance(u, User)
来源：http://qmq.hnqzz.top

PHP:  $u instanceof User
来源：http://swy.jyoumei.cn

JS:   u instanceof User
来源：http://zqn.yj202588.top

TS:   u instanceof User
来源：http://mpz.zdbjq.cn

Java: u instanceof User
来源：http://ixp.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dzz.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://gwe.birdmap.top

C#:   u is User
来源：http://byz.sxryk.cn

[G14] 数据类 / record
来源：http://wbu.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ale.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://cbp.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://ywh.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://doq.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://kxa.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://fbl.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hwv.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://dvu.nanxinkj.top

[G15] 枚举
来源：http://dcy.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rpi.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fbz.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wdq.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ltw.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://lqe.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tyh.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://vvz.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nnx.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://vds.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://avg.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://cni.aibaodan.cn

JS:   Object.entries(obj)
来源：http://wss.gzhubu.top

TS:   Object.entries(obj)
来源：http://ika.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uby.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://epi.zhengqikj.top

Ruby: obj.instance_variables
来源：http://xht.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://pkc.jinyuanbaomall.cn

================================================================================
来源：http://upb.sjlbkw.cn

H. 异常与错误处理
来源：http://cje.yuxming.cn

================================================================================
来源：http://std.yanxiufei.cn

[H01] try / catch 基础
来源：http://gzv.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iov.hnxiangtu.top


<!-- 参考信息 -->