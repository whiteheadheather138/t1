代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oxe.daxiang520.top

[E19] 多行文本按行拆分
来源：http://fqg.vehdjk.com

Py:   s.splitlines()
来源：http://cdg.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fey.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://jva.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://ojn.yvedp.cn

Java: s.lines().toList()
来源：http://ibh.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://knv.zhiwuduotai.top

Ruby: s.lines
来源：http://ohm.chenzaomai.com

C#:   s.Split('\n')
来源：http://ylp.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://mtm.yfazqb.com

Py:   if not s:
来源：http://tif.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oov.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qoo.guowangkeji.top

TS:   if (s === "") {}
来源：http://wye.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://xig.dianchejie.cn

Go:   if s == "" {}
来源：http://lgb.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://ybb.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gwu.redwolf501.top

[E21] 超长截断加省略号
来源：http://epl.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wer.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://npo.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yug.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bob.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jpf.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://fop.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cph.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kut.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://bed.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fwg.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sel.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lpw.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyj.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ewk.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fpp.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://rlg.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zuq.pengpengdd.cyou

================================================================================
来源：http://jdw.fehbvm.com

F. 文件与目录
来源：http://qhd.jinqigfzy.top

================================================================================
来源：http://ryk.jiagoushi.top

[F01] 读取整个文件
来源：http://rsz.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://byh.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://lpa.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqc.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mox.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://twm.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gug.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://cap.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://ttc.316326.xyz

[F02] 逐行读取文件
来源：http://kkj.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mnu.zhixingplan.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rgd.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://puz.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llf.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ohb.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zsq.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fjs.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gto.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://gww.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vix.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wbx.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qsq.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smd.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ebt.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://krx.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://mhw.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ilq.gogol.net.cn

[F04] 追加写入文件
来源：http://ygz.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://alg.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fea.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aeb.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://int.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uje.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bdz.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://idl.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://htq.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://upr.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pvg.yj20258.top

PHP:  file_exists("a.txt");
来源：http://llc.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://hmu.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://tjw.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vob.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kpy.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://xfa.hysaishi.cn

C#:   File.Exists("a.txt")
来源：http://mfu.zhiwuduotai.top

[F06] 删除文件
来源：http://uuy.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://kcj.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://pbg.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://wyu.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://vqa.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://obp.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://pfx.316326.xyz

Ruby: File.delete("a.txt")
来源：http://hlm.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://ynz.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://fre.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bzk.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nvz.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cnn.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qfc.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dmh.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yyf.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gbl.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fhv.redwolf501.top

[F08] 遍历目录
来源：http://kbw.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oiu.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ytb.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://rdk.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://roz.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jld.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vjo.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://fbm.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://jkv.sweek.top

[F09] 获取文件大小
来源：http://aju.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://oio.sweek.top

PHP:  filesize("a.txt");
来源：http://tuv.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://ylt.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://gxg.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eqi.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxf.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://htt.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://jwl.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://qmy.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kfa.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://odg.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mpd.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://oqi.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bfi.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sdp.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wlm.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://war.tarul.cn

[F11] 复制与移动文件
来源：http://foz.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yal.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oon.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://thy.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivv.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zfc.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://azl.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gef.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tyz.sjlbkw.cn

[F12] CSV 读写
来源：http://jlw.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iqe.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vre.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kqb.yanxiufei.cn

TS:   // 同上
来源：http://rhr.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tkn.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kzp.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://edb.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uix.hfpthk.cn

================================================================================
来源：http://sjm.tian-w.cn

G. 面向对象
来源：http://cxh.hcnkem.com

================================================================================
来源：http://hfl.316326.xyz

[G01] 定义类
来源：http://poh.jinyuanbaomall.cn

Py:   class User: pass
来源：http://omd.nwbrower.top

PHP:  class User {}
来源：http://eab.feifeiyinyue.top

JS:   class User {}
来源：http://bsj.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://ejt.shanyushiyangtech.top

Java: class User {}
来源：http://xnc.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://yiy.zhaomingkeji.xyz

Ruby: class User; end
来源：http://fig.hywenlv.cn

C#:   class User {}
来源：http://jtg.ywan-chungtsiang.top

[G02] 构造函数
来源：http://yoo.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xbv.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://xqz.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://kiz.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://jfa.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://fnk.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mdv.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://iaf.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://lpe.haohaochexian.top

[G03] 实例属性
来源：http://ptm.tarul.cn

Py:   self.name = "x"
来源：http://nnc.pycfn.com

PHP:  public string $name = "x";
来源：http://wte.0kj1m.cn

JS:   this.name = "x";
来源：http://cjc.mhx1999.top

TS:   name: string = "x";
来源：http://rxv.vehdjk.com

Java: private String name;
来源：http://cqs.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pkq.aibaodan.cn

Ruby: @name = "x"
来源：http://ume.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://aor.redwolf501.top

[G04] 定义方法
来源：http://wui.cashguo.top

Py:   def greet(self): return self.name
来源：http://htk.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://bne.yj202588.top

JS:   greet() { return this.name; }
来源：http://rdd.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://rvq.sweek.top

Java: String greet() { return name; }
来源：http://ush.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ars.hcnkem.com

Ruby: def greet; @name; end
来源：http://pek.hnqzz.top

C#:   public string Greet() => Name;
来源：http://mdi.hesvh.cn

[G05] 继承
来源：http://plo.chenzaomai.com

Py:   class Admin(User): pass
来源：http://qgq.jianghu66.top

PHP:  class Admin extends User {}
来源：http://ssc.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://nly.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://ltx.haohaochexian.top

Java: class Admin extends User {}
来源：http://rhr.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pqo.jqgfzy.top

Ruby: class Admin < User; end
来源：http://jxh.hywenlv.cn

C#:   class Admin : User {}
来源：http://fmw.xziqi.cn

[G06] 重写方法
来源：http://gux.birdmap.top

Py:   def greet(self): return "admin"
来源：http://wod.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gpk.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://umx.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://sxq.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://hqm.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgd.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://tbh.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://bxs.svipenyu.cn

[G07] 调用父类方法
来源：http://eqq.zhengqikj.top

Py:   super().greet()
来源：http://rxq.tianlin.xyz

PHP:  parent::greet();
来源：http://cwe.yangfankeji.com

JS:   super.greet();
来源：http://ufr.zdqjudy.top

TS:   super.greet();
来源：http://amy.ppjwa.cn

Java: super.greet();
来源：http://stv.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vfd.sufxvd.cn

Ruby: super
来源：http://spp.fktsv.cn

C#:   base.Greet();
来源：http://fip.meibo888.top

[G08] 静态方法与属性
来源：http://oet.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nmm.cheryme.top

PHP:  public static function f() {}
来源：http://abk.guannengcc.top

JS:   static f() {}
来源：http://tqp.hfpthk.cn

TS:   static f(): void {}
来源：http://kdh.chenjidiqi.icu

Java: static void f() {}
来源：http://apy.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://lkw.havefunace.top

Ruby: def self.f; end
来源：http://mgb.sysykeji.top

C#:   public static void F() {}
来源：http://pry.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://bdm.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://myy.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://ycq.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hkj.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://bwd.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://mbz.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://oyd.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wzz.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://uaf.yj202588.top

[G10] 访问控制
来源：http://pws.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://qvw.jqgufenzy.top

PHP:  public / protected / private
来源：http://rco.yonumen.top

JS:   #private 字段；其余公开
来源：http://eyb.zhiwuduotai.top

TS:   public / protected / private
来源：http://xpt.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://kgc.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://tos.yfazqb.com

Ruby: public / protected / private
来源：http://ygd.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://trg.yonumen.top

[G11] getter / setter
来源：http://nnd.iojbl.cn

Py:   @property 与 @x.setter
来源：http://klf.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tvc.fzhhl.top

JS:   get name() { return this._name; }
来源：http://trk.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://bie.hammf.cn

Java: public String getName() { return name; }
来源：http://ukf.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uxi.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://avz.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://pxp.chenlongwang.top

[G12] 对象转字符串
来源：http://opw.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://ovl.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://xdr.bjfxy.top

JS:   toString() { return this.name; }
来源：http://xrs.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://jnm.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://edc.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://ckn.tanke756.top

Ruby: def to_s; @name; end
来源：http://kgg.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://iwx.cashguo.top

[G13] 判断对象类型
来源：http://twj.tianlin.xyz

Py:   isinstance(u, User)
来源：http://glj.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://zhq.yvedp.cn

JS:   u instanceof User
来源：http://sab.gotoacloud.top

TS:   u instanceof User
来源：http://gxn.jinyuanbaomall.cn

Java: u instanceof User
来源：http://piu.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qoi.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://xqm.xinyue.icu

C#:   u is User
来源：http://iaz.aibaodan.cn

[G14] 数据类 / record
来源：http://ydf.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qhb.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://wgi.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://hun.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://tdx.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://wub.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://gwb.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tkl.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://jrk.ehwqpu.com

[G15] 枚举
来源：http://bui.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lgt.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bva.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vup.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zma.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://cjm.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dew.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://kui.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lql.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://dgo.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwp.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://niv.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://lah.mhx1999.top

TS:   Object.entries(obj)
来源：http://jmw.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lhu.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rik.fehbvm.com

Ruby: obj.instance_variables
来源：http://ykc.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://zec.fanxiaobao.xyz

================================================================================
来源：http://msh.haohaochexian.top

H. 异常与错误处理
来源：http://okf.shzxlz.cn

================================================================================
来源：http://ztp.52xcode.cn

[H01] try / catch 基础
来源：http://gyf.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dta.ydjk.org.cn


<!-- 参考信息 -->