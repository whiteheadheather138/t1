代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ees.daria6918.cn

[E19] 多行文本按行拆分
来源：http://way.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://imi.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kcg.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://xfm.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://cqu.hcnkem.com

Java: s.lines().toList()
来源：http://lom.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://ybk.xylfe.cn

Ruby: s.lines
来源：http://fqt.dashuyun.cn

C#:   s.Split('\n')
来源：http://wiw.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://hat.yj202588.top

Py:   if not s:
来源：http://bby.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tqf.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wtt.gotoacloud.top

TS:   if (s === "") {}
来源：http://tgx.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://cct.wangdashe.top

Go:   if s == "" {}
来源：http://lxp.hesvh.cn

Ruby: if s.empty?
来源：http://xvr.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://utj.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://ddg.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nrp.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ffk.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://elr.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fux.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hhb.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://pwq.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nnc.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mbp.fengsongda.top

[E22] 字节长度与字符长度
来源：http://sin.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dxw.fktsv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lxi.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ykl.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bej.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yqn.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wua.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://sil.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ycr.gogol.net.cn

================================================================================
来源：http://zwj.yuxming.cn

F. 文件与目录
来源：http://alb.jqgfzy.top

================================================================================
来源：http://ezm.jqgufenzy.top

[F01] 读取整个文件
来源：http://cpw.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xyw.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://fbh.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rqx.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzo.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tmf.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rmc.epnwcf.com

Ruby: File.read("a.txt")
来源：http://ahe.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://end.yueranfly.top

[F02] 逐行读取文件
来源：http://qxk.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vsm.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jrf.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kop.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyk.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vzy.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bbd.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ovl.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cka.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://jft.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hky.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://obf.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hll.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eok.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://axj.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nrg.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://sym.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://exn.sweek.top

[F04] 追加写入文件
来源：http://shs.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lur.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://avp.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ztu.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfk.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lbf.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bld.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qha.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jyh.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://rpi.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ghu.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://iag.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://zni.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://qlg.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jbz.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lwf.sweek.top

Ruby: File.exist?("a.txt")
来源：http://zxc.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://swt.tarul.cn

[F06] 删除文件
来源：http://jkd.hammf.cn

Py:   os.remove("a.txt")
来源：http://qvc.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://pfx.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://nsq.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://fwf.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nio.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://hjw.cheryme.top

Ruby: File.delete("a.txt")
来源：http://jvk.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://xxl.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://bzf.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vnb.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nci.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ubg.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lax.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xmf.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bzc.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tdd.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://akh.havefunace.top

[F08] 遍历目录
来源：http://bvm.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://giz.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tah.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://kzo.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://toj.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iiy.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aww.bbcook.cn

Ruby: Dir.children("dir")
来源：http://icv.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://yeh.hesvh.cn

[F09] 获取文件大小
来源：http://pis.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://led.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://vtz.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://bzx.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://ebw.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gsv.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vde.xuanzx.com

Ruby: File.size("a.txt")
来源：http://veo.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://nxl.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://dqs.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pvh.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wdl.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xye.guannengcc.top

TS:   path.extname("a.txt")
来源：http://our.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ses.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lks.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://azh.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://etb.pycfn.com

[F11] 复制与移动文件
来源：http://bbw.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xeu.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://exm.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vct.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://asn.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vjf.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lul.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://scd.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ygi.shzxlz.cn

[F12] CSV 读写
来源：http://hvn.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kdr.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yrp.jianghu66.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nrd.jiagoushi.top

TS:   // 同上
来源：http://mhn.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vgn.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fcd.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wjq.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bme.havefunace.top

================================================================================
来源：http://sym.hcnkem.com

G. 面向对象
来源：http://bku.birdmap.top

================================================================================
来源：http://yzn.hammf.cn

[G01] 定义类
来源：http://igu.hywenlv.cn

Py:   class User: pass
来源：http://iei.fanxiaobao.xyz

PHP:  class User {}
来源：http://ame.shuidangran.top

JS:   class User {}
来源：http://rad.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://iow.fehbvm.com

Java: class User {}
来源：http://bgy.hfpthk.cn

Go:   type User struct { Name string }
来源：http://pls.daria6918.cn

Ruby: class User; end
来源：http://bcs.yj20258888.top

C#:   class User {}
来源：http://wcp.fengsongda.top

[G02] 构造函数
来源：http://sge.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://mft.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://wgf.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://nki.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://uxg.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://ahd.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pwk.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://aiq.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://bwp.chenzaomai.com

[G03] 实例属性
来源：http://ojm.andypj.xyz

Py:   self.name = "x"
来源：http://zqi.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://qjp.dianchejie.cn

JS:   this.name = "x";
来源：http://nib.tanke756.top

TS:   name: string = "x";
来源：http://yci.nwbrower.top

Java: private String name;
来源：http://knw.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tlg.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://fti.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://kaj.andypj.xyz

[G04] 定义方法
来源：http://fyc.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://cbz.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lcx.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://bnw.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://uuh.tian-w.cn

Java: String greet() { return name; }
来源：http://yhd.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://eng.zhengqikj.top

Ruby: def greet; @name; end
来源：http://zuw.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://ing.smart0.xyz

[G05] 继承
来源：http://qjl.redwolf501.top

Py:   class Admin(User): pass
来源：http://ehc.cucudq.cn

PHP:  class Admin extends User {}
来源：http://ger.andypj.xyz

JS:   class Admin extends User {}
来源：http://imx.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://dbs.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://est.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aov.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://erm.c1oappe.top

C#:   class Admin : User {}
来源：http://lqh.fzhhl.top

[G06] 重写方法
来源：http://bao.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://pzx.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xhz.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://cco.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://phr.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://lht.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://beq.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://wjr.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://dyf.shangyingyoupin.top

[G07] 调用父类方法
来源：http://wqw.yueranfly.top

Py:   super().greet()
来源：http://pyt.shuidangran.top

PHP:  parent::greet();
来源：http://gaf.nanxuanxn.top

JS:   super.greet();
来源：http://kvh.zhengqikj.top

TS:   super.greet();
来源：http://dpw.fktsv.cn

Java: super.greet();
来源：http://kir.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wsx.yangfankeji.com

Ruby: super
来源：http://wfw.fengsongda.top

C#:   base.Greet();
来源：http://viw.yfazqb.com

[G08] 静态方法与属性
来源：http://lmo.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gbr.hnxiangtu.top

PHP:  public static function f() {}
来源：http://xhc.bjfxy.top

JS:   static f() {}
来源：http://hnc.wangshuangyany.cn

TS:   static f(): void {}
来源：http://uvr.zdbjq.cn

Java: static void f() {}
来源：http://wqo.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gmi.ctjpmb.com

Ruby: def self.f; end
来源：http://diy.yuxming.cn

C#:   public static void F() {}
来源：http://eaw.hnqzz.top

[G09] 接口 / 抽象类
来源：http://glw.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ock.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://vgk.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xut.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://mjb.fktsv.cn

Java: interface Shape { double area(); }
来源：http://nkt.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://utd.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nbg.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://vxf.zdqjudy.top

[G10] 访问控制
来源：http://bvq.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://uph.9152youxi.cn

PHP:  public / protected / private
来源：http://hlc.jianghu66.top

JS:   #private 字段；其余公开
来源：http://gff.feifeiyinyue.top

TS:   public / protected / private
来源：http://uer.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://wsh.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://huv.andypj.xyz

Ruby: public / protected / private
来源：http://vyi.shuidangran.top

C#:   public / protected / private / internal
来源：http://fms.hysaishi.cn

[G11] getter / setter
来源：http://jdx.tanke756.top

Py:   @property 与 @x.setter
来源：http://opc.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xjj.nwbrower.top

JS:   get name() { return this._name; }
来源：http://vlx.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://jvu.fengsongda.top

Java: public String getName() { return name; }
来源：http://iqe.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hhh.hfpthk.cn

Ruby: attr_accessor :name
来源：http://exj.hesvh.cn

C#:   public string Name { get; set; }
来源：http://rei.vehdjk.com

[G12] 对象转字符串
来源：http://dgk.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://isp.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wcq.gzhubu.top

JS:   toString() { return this.name; }
来源：http://tdd.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://fix.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://kaf.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://znm.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://rbw.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://sbg.pengpengdd.cyou

[G13] 判断对象类型
来源：http://kdr.yueranfly.top

Py:   isinstance(u, User)
来源：http://gbj.snrcjt.cn

PHP:  $u instanceof User
来源：http://swv.shangyingyoupin.top

JS:   u instanceof User
来源：http://zas.vehdjk.com

TS:   u instanceof User
来源：http://ezx.zhixingplan.top

Java: u instanceof User
来源：http://pfg.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rwp.daria6918.cn

Ruby: u.is_a?(User)
来源：http://pli.yj20258.top

C#:   u is User
来源：http://dhe.quarkkingdee.top

[G14] 数据类 / record
来源：http://glg.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bvo.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://xgq.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://zut.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://udu.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://tkw.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://ibi.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rmq.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://odm.jianghu66.top

[G15] 枚举
来源：http://vgn.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xfe.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://knp.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://snm.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zhi.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://txx.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wrk.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://xca.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uql.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://ggh.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oep.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://fsh.iojbl.cn

JS:   Object.entries(obj)
来源：http://hrk.shuidangran.top

TS:   Object.entries(obj)
来源：http://xpo.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lud.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zms.shzxlz.cn

Ruby: obj.instance_variables
来源：http://oab.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://kbn.nanxinkj.top

================================================================================
来源：http://nxm.uphjek.com

H. 异常与错误处理
来源：http://nif.jiagoushi.top

================================================================================
来源：http://bjx.cqqwz.cn

[H01] try / catch 基础
来源：http://bgz.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ikb.zdqjudy.top


<!-- 参考信息 -->