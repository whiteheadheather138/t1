代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://ckm.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://diq.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ube.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfg.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qoc.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://yyd.daria6918.cn

Py:   s.splitlines()
来源：http://dos.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sam.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://yun.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://nvl.sweek.top

Java: s.lines().toList()
来源：http://atr.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://ybo.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://mfs.bjfxy.top

C#:   s.Split('\n')
来源：http://ttz.pycfn.com

[E20] 判断字符串是否为空
来源：http://osb.ydjk.org.cn

Py:   if not s:
来源：http://eig.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uap.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bzv.sweek.top

TS:   if (s === "") {}
来源：http://nkt.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://gxj.hywenlv.cn

Go:   if s == "" {}
来源：http://boj.sxryk.cn

Ruby: if s.empty?
来源：http://crp.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://csr.ppjwa.cn

[E21] 超长截断加省略号
来源：http://dyd.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eyy.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gbu.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cas.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxj.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ddo.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://qlr.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cqy.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sbv.shuidangran.top

[E22] 字节长度与字符长度
来源：http://vpm.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://agc.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://beo.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwa.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nlc.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lox.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mqb.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://iap.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rvo.c1oappe.top

================================================================================
来源：http://rhg.ivvv.top

F. 文件与目录
来源：http://ynu.andypj.xyz

================================================================================
来源：http://nar.hnqzz.top

[F01] 读取整个文件
来源：http://xol.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uae.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://grh.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ivs.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zvx.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ygt.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nri.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://bzi.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://uuj.yvedp.cn

[F02] 逐行读取文件
来源：http://jwx.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sut.jinqigufen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rzl.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mog.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fiw.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kpy.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tjy.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://myi.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bwv.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://kqx.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sbo.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://qux.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://woa.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fjk.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tdi.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nke.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://bnx.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tsh.zdqjudy.top

[F04] 追加写入文件
来源：http://rfx.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gss.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qrq.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iao.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qym.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dkq.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://czj.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://chf.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dnx.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://gkg.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kfh.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://rnn.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://yqv.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://rxw.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://obe.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://twc.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://vjh.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://fdr.cucudq.cn

[F06] 删除文件
来源：http://aga.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://ocu.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://pog.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://uef.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://lpt.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uds.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://edo.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://gsf.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://pzs.yj202588.top

[F07] 创建目录（含多级）
来源：http://smp.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oiy.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vhr.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqd.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hid.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dbg.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vvb.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gri.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dae.hcnkem.com

[F08] 遍历目录
来源：http://sti.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ayc.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kfe.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://ydo.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://vsm.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oqs.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qad.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://xrj.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://grs.0kj1m.cn

[F09] 获取文件大小
来源：http://dlz.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://yrb.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://kud.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://sre.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://rin.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://zai.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gqs.smart0.xyz

Ruby: File.size("a.txt")
来源：http://cut.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://fep.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://zcr.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vfo.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tzq.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oru.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://jtu.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://omv.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tzu.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bsq.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://irr.yangfankeji.com

[F11] 复制与移动文件
来源：http://ful.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jbq.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://red.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pws.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jvz.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uaj.birdmap.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://enr.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xol.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uxv.feifeiyinyue.top

[F12] CSV 读写
来源：http://osz.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cnq.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oti.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uay.gaohongyu789.top

TS:   // 同上
来源：http://vgm.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nvh.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kmm.guowangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vrg.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://gbh.cashguo.top

================================================================================
来源：http://yfc.yj202588.top

G. 面向对象
来源：http://dji.zdbjq.cn

================================================================================
来源：http://dta.hesvh.cn

[G01] 定义类
来源：http://sed.jqgfzy.top

Py:   class User: pass
来源：http://qht.gaohongyu789.top

PHP:  class User {}
来源：http://nlq.ivvv.top

JS:   class User {}
来源：http://asw.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://hvb.yonumen.top

Java: class User {}
来源：http://eua.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://kjy.zdqjudy.top

Ruby: class User; end
来源：http://xpi.vehdjk.com

C#:   class User {}
来源：http://gty.chenzaomai.com

[G02] 构造函数
来源：http://hpm.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://cyq.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://neq.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://pwn.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://tad.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://oae.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oiu.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://qex.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://ias.shangyingyoupin.top

[G03] 实例属性
来源：http://fgw.cheryme.top

Py:   self.name = "x"
来源：http://krj.jinqigufen.top

PHP:  public string $name = "x";
来源：http://vkx.shangyingyoupin.top

JS:   this.name = "x";
来源：http://pzz.xinyue.icu

TS:   name: string = "x";
来源：http://apv.tanke756.top

Java: private String name;
来源：http://hhu.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yit.hesvh.cn

Ruby: @name = "x"
来源：http://kmb.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://paq.feifeiyinyue.top

[G04] 定义方法
来源：http://mqd.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://waj.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ncz.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://psd.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://fpn.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://kag.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tlh.cqqwz.cn

Ruby: def greet; @name; end
来源：http://zfj.mhx1999.top

C#:   public string Greet() => Name;
来源：http://gwf.chenjidiqi.icu

[G05] 继承
来源：http://qlg.mhx1999.top

Py:   class Admin(User): pass
来源：http://hkz.fehbvm.com

PHP:  class Admin extends User {}
来源：http://xhg.yonumen.top

JS:   class Admin extends User {}
来源：http://ssp.xylfe.cn

TS:   class Admin extends User {}
来源：http://isg.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://jge.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vab.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://xid.epnwcf.com

C#:   class Admin : User {}
来源：http://lgr.jinqigufen.top

[G06] 重写方法
来源：http://hhj.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://mjq.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qwx.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://eug.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://hta.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://zua.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vjq.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://urc.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://jqd.bjfxy.top

[G07] 调用父类方法
来源：http://gqo.ppjwa.cn

Py:   super().greet()
来源：http://woz.snrcjt.cn

PHP:  parent::greet();
来源：http://gpz.epnwcf.com

JS:   super.greet();
来源：http://uda.pycfn.com

TS:   super.greet();
来源：http://sbw.zhixingplan.top

Java: super.greet();
来源：http://dts.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tkk.gogol.net.cn

Ruby: super
来源：http://vme.sweek.top

C#:   base.Greet();
来源：http://rgw.dashuyun.cn

[G08] 静态方法与属性
来源：http://yiy.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zqt.yanxiufei.cn

PHP:  public static function f() {}
来源：http://tpo.cashguo.top

JS:   static f() {}
来源：http://pct.ydjk.org.cn

TS:   static f(): void {}
来源：http://atp.jlsjyb.cn

Java: static void f() {}
来源：http://bzw.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gav.redwolf501.top

Ruby: def self.f; end
来源：http://jud.pengpengdd.cyou

C#:   public static void F() {}
来源：http://hyu.tarul.cn

[G09] 接口 / 抽象类
来源：http://kkw.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://iwv.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://gyi.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nqm.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://fgg.tian-w.cn

Java: interface Shape { double area(); }
来源：http://ske.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://mql.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kah.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://gpx.daxiang520.top

[G10] 访问控制
来源：http://xij.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://mee.cashguo.top

PHP:  public / protected / private
来源：http://aeo.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://lrl.zhiwuduotai.top

TS:   public / protected / private
来源：http://lji.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://sgg.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ovx.hnqzz.top

Ruby: public / protected / private
来源：http://gaw.yuxming.cn

C#:   public / protected / private / internal
来源：http://mrs.jinghuilouyu.cn

[G11] getter / setter
来源：http://fwv.tarul.cn

Py:   @property 与 @x.setter
来源：http://ryn.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://ozw.ybcxt.top

JS:   get name() { return this._name; }
来源：http://omo.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://roo.epnwcf.com

Java: public String getName() { return name; }
来源：http://zml.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mmy.hywenlv.cn

Ruby: attr_accessor :name
来源：http://uvt.tanke756.top

C#:   public string Name { get; set; }
来源：http://cta.bjfxy.top

[G12] 对象转字符串
来源：http://pwf.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://ilw.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qxn.redwolf501.top

JS:   toString() { return this.name; }
来源：http://fql.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://gzn.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://wqg.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://deu.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://ixt.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://qng.cqqwz.cn

[G13] 判断对象类型
来源：http://tdo.aibaodan.cn

Py:   isinstance(u, User)
来源：http://mfk.wangdashe.top

PHP:  $u instanceof User
来源：http://xrf.yfazqb.com

JS:   u instanceof User
来源：http://dqo.gogol.net.cn

TS:   u instanceof User
来源：http://xkl.nanxinkj.top

Java: u instanceof User
来源：http://phf.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pgl.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://elm.vqdsnc.cn

C#:   u is User
来源：http://yqy.9152youxi.cn

[G14] 数据类 / record
来源：http://kfb.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://enf.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://tah.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://qwn.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://bwb.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://qau.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://rnw.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wnp.hammf.cn

C#:   record User(string Name, int Age);
来源：http://ske.yangfankeji.com

[G15] 枚举
来源：http://pje.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pzx.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cqu.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://evf.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ors.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://phb.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ocv.chenjidiqi.icu

Ruby: Color = %i[red green].freeze
来源：http://iuj.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://agk.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://sty.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wbg.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://fmj.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://guw.yfazqb.com

TS:   Object.entries(obj)
来源：http://wnj.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qxu.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hft.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://bpu.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://owi.hfpthk.cn

================================================================================
来源：http://aka.kuanghao11.cn


<!-- 参考信息 -->