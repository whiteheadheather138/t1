代发 wailian999

[E18] 模板占位符替换
来源：http://auu.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wto.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://njt.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ovo.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qsk.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://muo.hongshengwenyu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mjh.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uum.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rdx.havefunace.top

[E19] 多行文本按行拆分
来源：http://sik.bjfxy.top

Py:   s.splitlines()
来源：http://zxi.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pqa.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://ljd.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://jjm.zhixingplan.top

Java: s.lines().toList()
来源：http://pyi.sweek.top

Go:   strings.Split(s, "\n")
来源：http://dtc.hesvh.cn

Ruby: s.lines
来源：http://khh.cdnleiting.top

C#:   s.Split('\n')
来源：http://sbn.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://jws.sweek.top

Py:   if not s:
来源：http://bjg.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bvp.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kuc.sysykeji.top

TS:   if (s === "") {}
来源：http://kuf.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://sfi.wangshuangyany.cn

Go:   if s == "" {}
来源：http://kde.hnqzz.top

Ruby: if s.empty?
来源：http://svq.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mkr.tianlin.xyz

[E21] 超长截断加省略号
来源：http://tsj.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mqx.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eyn.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://odd.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://akd.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://goh.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://ubj.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xcc.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kep.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://xke.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nwx.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hcp.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmv.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gtr.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ptz.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://art.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://mkc.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wzu.yuxming.cn

================================================================================
来源：http://waj.chenzaomai.com

F. 文件与目录
来源：http://pus.chenjidiqi.icu

================================================================================
来源：http://yli.daria6918.cn

[F01] 读取整个文件
来源：http://cup.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nfu.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://psg.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://drv.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nua.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jus.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://beo.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://yzs.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://yqa.yuxming.cn

[F02] 逐行读取文件
来源：http://jqv.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mdx.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vnq.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dkx.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://znw.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lle.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://moj.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bke.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xdi.yj20258.top

[F03] 写入文件（覆盖）
来源：http://wmo.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vny.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://vnz.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kit.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://avp.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wqw.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tac.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://cpk.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lse.yj20258.top

[F04] 追加写入文件
来源：http://bvz.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wjm.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xna.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nbd.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rsf.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zwf.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qis.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mly.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://irp.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://ier.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hph.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://tpi.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://rof.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://jrn.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tnl.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ctc.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://vql.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://jsu.yuanzhike.top

[F06] 删除文件
来源：http://nmy.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://xvs.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://zgo.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://riv.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yzq.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mbh.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://juo.sweek.top

Ruby: File.delete("a.txt")
来源：http://grk.meibo888.top

C#:   File.Delete("a.txt");
来源：http://llr.daria6918.cn

[F07] 创建目录（含多级）
来源：http://akq.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bpq.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gyl.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rwy.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ncj.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hzq.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ufb.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ujx.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xhb.ehwqpu.com

[F08] 遍历目录
来源：http://hwz.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nlk.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vno.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://yrv.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://jjp.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bae.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mgi.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://ytt.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://dwt.hesvh.cn

[F09] 获取文件大小
来源：http://mdc.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://rqi.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://ygr.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://spx.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://fdj.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cvu.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lrd.havefunace.top

Ruby: File.size("a.txt")
来源：http://ayv.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://goc.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://xhd.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wgw.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oyc.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ixv.ydzc1.top

TS:   path.extname("a.txt")
来源：http://fpp.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cme.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aku.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://evh.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ulg.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://rcd.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qrv.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qcw.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jkw.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qgi.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dur.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://viy.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nbf.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kkt.gzhubu.top

[F12] CSV 读写
来源：http://igx.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bit.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sta.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nei.guowangkeji.top

TS:   // 同上
来源：http://ryl.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dtq.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wvr.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://exl.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rxh.ctjpmb.com

================================================================================
来源：http://riw.xinyue.icu

G. 面向对象
来源：http://hln.fehbvm.com

================================================================================
来源：http://rhq.bbcook.cn

[G01] 定义类
来源：http://ccs.vqdsnc.cn

Py:   class User: pass
来源：http://zen.aizwys.cn

PHP:  class User {}
来源：http://ebo.ydjk.org.cn

JS:   class User {}
来源：http://yqv.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://tzu.jianghu66.top

Java: class User {}
来源：http://ohb.ivvv.top

Go:   type User struct { Name string }
来源：http://tlj.0kj1m.cn

Ruby: class User; end
来源：http://udf.kuanghao11.cn

C#:   class User {}
来源：http://pkl.ppjwa.cn

[G02] 构造函数
来源：http://bsq.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://xet.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://kae.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://ika.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://dcq.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://lxm.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jfk.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://bfs.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://lnp.ehwqpu.com

[G03] 实例属性
来源：http://vvh.jiagoushi.top

Py:   self.name = "x"
来源：http://psp.52xcode.cn

PHP:  public string $name = "x";
来源：http://ool.vehdjk.com

JS:   this.name = "x";
来源：http://qbh.c1oappe.top

TS:   name: string = "x";
来源：http://slf.mhx1999.top

Java: private String name;
来源：http://kez.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sge.ehwqpu.com

Ruby: @name = "x"
来源：http://tbd.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://ldw.daria6918.cn

[G04] 定义方法
来源：http://aiy.havefunace.top

Py:   def greet(self): return self.name
来源：http://zst.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://epb.hammf.cn

JS:   greet() { return this.name; }
来源：http://dze.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://nyb.cucudq.cn

Java: String greet() { return name; }
来源：http://ulw.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://vju.yj20258.top

Ruby: def greet; @name; end
来源：http://itu.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://yss.sweek.top

[G05] 继承
来源：http://rht.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://dpo.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://zao.bjfxy.top

JS:   class Admin extends User {}
来源：http://oqj.tian-w.cn

TS:   class Admin extends User {}
来源：http://bgo.cucudq.cn

Java: class Admin extends User {}
来源：http://cxf.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qjg.zdqjudy.top

Ruby: class Admin < User; end
来源：http://xkv.zhengqikj.top

C#:   class Admin : User {}
来源：http://eln.tarul.cn

[G06] 重写方法
来源：http://pfc.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://uad.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fdn.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://yjh.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://fdd.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://xre.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://exo.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://ysh.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://wtw.epnwcf.com

[G07] 调用父类方法
来源：http://lmr.fzhhl.top

Py:   super().greet()
来源：http://cne.316326.xyz

PHP:  parent::greet();
来源：http://wko.sjlbkw.cn

JS:   super.greet();
来源：http://ipc.hesvh.cn

TS:   super.greet();
来源：http://ktg.shangyingyoupin.top

Java: super.greet();
来源：http://swl.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ktx.xziqi.cn

Ruby: super
来源：http://gat.zdqjudy.top

C#:   base.Greet();
来源：http://gxk.fzhhl.top

[G08] 静态方法与属性
来源：http://nde.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lvd.hnxiangtu.top

PHP:  public static function f() {}
来源：http://uud.hfpthk.cn

JS:   static f() {}
来源：http://gto.sufxvd.cn

TS:   static f(): void {}
来源：http://hye.zhoulong.xyz

Java: static void f() {}
来源：http://pqn.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bkc.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://nwc.wangshuangyany.cn

C#:   public static void F() {}
来源：http://yoo.ybcxt.top

[G09] 接口 / 抽象类
来源：http://slp.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://qij.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://epa.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zey.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://ois.hesvh.cn

Java: interface Shape { double area(); }
来源：http://szn.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://tbi.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xfh.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://wll.ppjwa.cn

[G10] 访问控制
来源：http://ehk.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://ait.52xcode.cn

PHP:  public / protected / private
来源：http://kcp.tian-w.cn

JS:   #private 字段；其余公开
来源：http://zha.xuetiantiany.cn

TS:   public / protected / private
来源：http://msc.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://sda.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nvn.yj20258888.top

Ruby: public / protected / private
来源：http://yeq.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://lil.pengpengdd.cyou

[G11] getter / setter
来源：http://hhb.fehbvm.com

Py:   @property 与 @x.setter
来源：http://pxc.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://trx.sweek.top

JS:   get name() { return this._name; }
来源：http://dmz.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://tal.bjfxy.top

Java: public String getName() { return name; }
来源：http://lzy.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ynn.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://fqe.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://hkv.gaohongyu789.top

[G12] 对象转字符串
来源：http://dbl.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://vui.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sco.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://dzp.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://hdk.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://vqr.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qmy.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://fry.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://hlx.meibo888.top

[G13] 判断对象类型
来源：http://jun.gotoacloud.top

Py:   isinstance(u, User)
来源：http://ukd.quarkkingdee.top

PHP:  $u instanceof User
来源：http://pba.quarkkingdee.top

JS:   u instanceof User
来源：http://nhs.guannengcc.top

TS:   u instanceof User
来源：http://dkj.hfpthk.cn

Java: u instanceof User
来源：http://lcq.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://csz.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://gjq.cheryme.top

C#:   u is User
来源：http://fuo.yongpay.top

[G14] 数据类 / record
来源：http://otq.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zbd.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://xax.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://rwx.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://vvf.cashguo.top

Java: record User(String name, int age) {}
来源：http://zdq.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://ggc.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lmq.birdmap.top

C#:   record User(string Name, int Age);
来源：http://rdl.fehbvm.com

[G15] 枚举
来源：http://age.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oia.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://coe.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nhb.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nuh.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://dqk.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qoi.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://sor.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://npn.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://tcu.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fod.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://epm.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://ema.daxiang520.top

TS:   Object.entries(obj)
来源：http://mgt.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qkl.fehbvm.com


<!-- 参考信息 -->