代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://kvo.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qud.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dqf.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://avs.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jyu.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://kxm.redwolf501.top

Py:   s.splitlines()
来源：http://ymx.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qkw.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://vwq.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://vec.yvedp.cn

Java: s.lines().toList()
来源：http://cjz.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://rll.kuanghao11.cn

Ruby: s.lines
来源：http://zsw.fktsv.cn

C#:   s.Split('\n')
来源：http://ult.tanke756.top

[E20] 判断字符串是否为空
来源：http://vmf.tanke756.top

Py:   if not s:
来源：http://zzq.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qbv.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pzc.shanyushiyangtech.top

TS:   if (s === "") {}
来源：http://dks.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://jyb.zhengqikj.top

Go:   if s == "" {}
来源：http://dro.hcnkem.com

Ruby: if s.empty?
来源：http://wml.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sft.iojbl.cn

[E21] 超长截断加省略号
来源：http://xot.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mci.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wvt.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dik.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uom.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dwb.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://jro.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://flx.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fsy.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://pgw.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vdq.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqf.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ptz.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bej.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oey.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tyu.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://uuw.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hir.tanke756.top

================================================================================
来源：http://pum.uphjek.com

F. 文件与目录
来源：http://jzk.fehbvm.com

================================================================================
来源：http://krr.yfazqb.com

[F01] 读取整个文件
来源：http://nuv.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tsc.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://dqg.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://acd.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://prz.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://myj.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://prs.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://ubo.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://jbv.chenzaomai.com

[F02] 逐行读取文件
来源：http://jly.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oos.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rde.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bnv.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vad.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gxf.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vjl.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zzg.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bag.havefunace.top

[F03] 写入文件（覆盖）
来源：http://vel.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://izz.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://hrz.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gtb.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vds.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dgz.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hoz.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://xdl.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jua.dashuyun.cn

[F04] 追加写入文件
来源：http://hnl.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zqw.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bas.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtd.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hil.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uou.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ceh.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awp.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://geq.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://bgt.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kgx.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://ywf.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://hfz.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://xiw.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rbt.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tuk.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://fkk.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://gms.316326.xyz

[F06] 删除文件
来源：http://ica.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://evd.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://opc.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://rtm.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://oox.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zce.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://pls.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://itt.yonumen.top

C#:   File.Delete("a.txt");
来源：http://evk.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://jkq.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://agc.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fvm.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qlt.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ncj.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://laq.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vmj.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://waj.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://omq.gaohongyu789.top

[F08] 遍历目录
来源：http://ycs.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://eum.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tcl.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://waw.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://lzy.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uzh.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://sqh.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://mvu.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://aqg.ydzc1.top

[F09] 获取文件大小
来源：http://pwl.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://zhr.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://luu.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://rgb.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://fab.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://imt.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nzh.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://azm.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://yyj.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://iam.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lwz.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bdt.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vkp.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://sbb.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dux.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jky.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hsq.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xkd.52xcode.cn

[F11] 复制与移动文件
来源：http://why.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cvw.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hml.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syn.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gno.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xng.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://woi.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hua.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://acc.iojbl.cn

[F12] CSV 读写
来源：http://bdv.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vdj.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uzd.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fqm.ybcxt.top

TS:   // 同上
来源：http://oje.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nqi.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://czx.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jht.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hio.zdbjq.cn

================================================================================
来源：http://shv.ppjwa.cn

G. 面向对象
来源：http://mtw.vqdsnc.cn

================================================================================
来源：http://mww.dashuyun.cn

[G01] 定义类
来源：http://ulf.yvedp.cn

Py:   class User: pass
来源：http://bbs.uphjek.com

PHP:  class User {}
来源：http://cvn.iojbl.cn

JS:   class User {}
来源：http://hrq.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://dct.yfazqb.com

Java: class User {}
来源：http://fii.jianghu66.top

Go:   type User struct { Name string }
来源：http://gje.pengpengdd.cyou

Ruby: class User; end
来源：http://rtl.sysykeji.top

C#:   class User {}
来源：http://yad.xziqi.cn

[G02] 构造函数
来源：http://ufl.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://krj.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://zqw.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://uqj.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://dvh.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://vza.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ppc.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://lsk.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://wxd.sweek.top

[G03] 实例属性
来源：http://sum.xinyue.icu

Py:   self.name = "x"
来源：http://ktt.ehwqpu.com

PHP:  public string $name = "x";
来源：http://dzi.hnqzz.top

JS:   this.name = "x";
来源：http://iru.hfpthk.cn

TS:   name: string = "x";
来源：http://xtb.jqgfzy.top

Java: private String name;
来源：http://hzz.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aio.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://ane.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://fdl.zhongyouzk.top

[G04] 定义方法
来源：http://sex.xziqi.cn

Py:   def greet(self): return self.name
来源：http://xst.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://wfn.hesvh.cn

JS:   greet() { return this.name; }
来源：http://rqw.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://dak.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://xye.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qvh.hesvh.cn

Ruby: def greet; @name; end
来源：http://sgp.hcnkem.com

C#:   public string Greet() => Name;
来源：http://eus.sweek.top

[G05] 继承
来源：http://ngu.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://nfw.xylfe.cn

PHP:  class Admin extends User {}
来源：http://agk.hnqzz.top

JS:   class Admin extends User {}
来源：http://vwr.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://byl.sufxvd.cn

Java: class Admin extends User {}
来源：http://nql.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://msz.svipenyu.cn

Ruby: class Admin < User; end
来源：http://zsx.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://tke.quarkkingdee.top

[G06] 重写方法
来源：http://sen.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://nmd.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ufz.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://sog.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://kdq.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://dok.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xme.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://ykj.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://eyv.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://gvr.jiagoushi.top

Py:   super().greet()
来源：http://tuy.sysykeji.top

PHP:  parent::greet();
来源：http://cdg.yj20258.top

JS:   super.greet();
来源：http://cfj.cashguo.top

TS:   super.greet();
来源：http://ati.daxiang520.top

Java: super.greet();
来源：http://zbx.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://miz.yonumen.top

Ruby: super
来源：http://arm.cucudq.cn

C#:   base.Greet();
来源：http://urw.epnwcf.com

[G08] 静态方法与属性
来源：http://edt.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hhz.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://hex.yueranfly.top

JS:   static f() {}
来源：http://jtj.jinqigfzy.top

TS:   static f(): void {}
来源：http://yha.zycfv.cn

Java: static void f() {}
来源：http://rwx.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://otg.fehbvm.com

Ruby: def self.f; end
来源：http://eip.sweek.top

C#:   public static void F() {}
来源：http://bdd.yueranfly.top

[G09] 接口 / 抽象类
来源：http://yny.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://ijd.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wrj.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ezb.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://cgu.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://uad.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://bhm.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eze.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://wvz.fktsv.cn

[G10] 访问控制
来源：http://gkk.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://vpp.9152youxi.cn

PHP:  public / protected / private
来源：http://nft.epnwcf.com

JS:   #private 字段；其余公开
来源：http://eeb.sysykeji.top

TS:   public / protected / private
来源：http://kwq.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://fvv.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jtv.dashuyun.cn

Ruby: public / protected / private
来源：http://dbx.tanke756.top

C#:   public / protected / private / internal
来源：http://vhw.hnxiangtu.top

[G11] getter / setter
来源：http://orj.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://xva.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://nzc.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://gxf.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://xxg.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://ebm.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ono.tarul.cn

Ruby: attr_accessor :name
来源：http://bcm.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://cbc.hcnkem.com

[G12] 对象转字符串
来源：http://fvm.cheryme.top

Py:   def __str__(self): return self.name
来源：http://gxe.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sbu.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://bqz.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://lwl.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://snj.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://drw.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://txc.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://fxc.zhiwuduotai.top

[G13] 判断对象类型
来源：http://kjp.guowangkeji.top

Py:   isinstance(u, User)
来源：http://qyo.sxryk.cn

PHP:  $u instanceof User
来源：http://xoc.sufxvd.cn

JS:   u instanceof User
来源：http://qyd.guowangkeji.top

TS:   u instanceof User
来源：http://rva.hfpthk.cn

Java: u instanceof User
来源：http://wyf.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sgv.cheryme.top

Ruby: u.is_a?(User)
来源：http://bhv.jianghu66.top

C#:   u is User
来源：http://olg.xziqi.cn

[G14] 数据类 / record
来源：http://nhq.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ugo.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://vcg.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://fce.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://dgf.zycfv.cn

Java: record User(String name, int age) {}
来源：http://zzo.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://adf.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yby.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://wbq.tarul.cn

[G15] 枚举
来源：http://gkt.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ijm.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://qem.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zzf.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bls.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://zia.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nit.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://whf.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wsv.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://cbf.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aat.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://ndm.xylfe.cn

JS:   Object.entries(obj)
来源：http://fcc.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://znk.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://leq.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cin.xylfe.cn

Ruby: obj.instance_variables
来源：http://nvt.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://ikl.aibaodan.cn

================================================================================
来源：http://dqv.andypj.xyz


<!-- 参考信息 -->