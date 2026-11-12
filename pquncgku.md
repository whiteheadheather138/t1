代发 wailian999

[E18] 模板占位符替换
来源：http://qmd.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pof.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://trl.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iqm.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://uft.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gsr.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wcn.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kyw.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rfu.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://jvp.chenjidiqi.icu

Py:   s.splitlines()
来源：http://dqh.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ahd.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://rmt.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://nso.gogol.net.cn

Java: s.lines().toList()
来源：http://hku.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://mpo.zhengqikj.top

Ruby: s.lines
来源：http://qql.xinyue.icu

C#:   s.Split('\n')
来源：http://hlw.fzhhl.top

[E20] 判断字符串是否为空
来源：http://xcp.ywan-chungtsiang.top

Py:   if not s:
来源：http://uld.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ird.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zxx.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://ywg.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://mds.jqgufenzy.top

Go:   if s == "" {}
来源：http://kuw.ehwqpu.com

Ruby: if s.empty?
来源：http://ltl.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ang.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://lnn.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pwy.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhb.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nee.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lyo.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nfo.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://rpw.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lbt.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vsv.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://fpm.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jwr.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zqp.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhh.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jge.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dwn.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bil.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://tmf.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jzw.aizwys.cn

================================================================================
来源：http://fyv.dashuyun.cn

F. 文件与目录
来源：http://nvq.hammf.cn

================================================================================
来源：http://iom.pengpengdd.cyou

[F01] 读取整个文件
来源：http://jdf.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yzk.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://jcj.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://axd.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ibc.iojbl.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qjj.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aiw.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://msx.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://nvh.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://lev.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mdo.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mgk.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://urj.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bes.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://liq.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vuv.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ibm.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qeu.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://jhl.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://brb.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vto.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bcl.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://noh.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pez.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eop.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://wtg.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kyq.yueranfly.top

[F04] 追加写入文件
来源：http://ajs.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zhc.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://upg.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqk.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eco.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://emw.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wze.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ses.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ace.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://nwd.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nub.yongpay.top

PHP:  file_exists("a.txt");
来源：http://qpb.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://ope.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://uhq.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gjw.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gbn.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://ovs.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://zny.pengpengdd.cyou

[F06] 删除文件
来源：http://evv.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://ofn.cashguo.top

PHP:  unlink("a.txt");
来源：http://qvi.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hkh.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://bvp.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vkf.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://vfp.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://tda.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://uea.cheryme.top

[F07] 创建目录（含多级）
来源：http://qwq.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nax.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ken.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xfa.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qkb.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vej.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eej.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ybt.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://epf.cheryme.top

[F08] 遍历目录
来源：http://qsu.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://xds.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://swa.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://vde.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://urp.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dkp.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tqz.yvedp.cn

Ruby: Dir.children("dir")
来源：http://ulz.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://gpk.hfpthk.cn

[F09] 获取文件大小
来源：http://yna.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://iad.xziqi.cn

PHP:  filesize("a.txt");
来源：http://hjj.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://ifr.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://amb.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lka.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ooj.52xcode.cn

Ruby: File.size("a.txt")
来源：http://gep.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://set.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://zyz.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gts.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ijc.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ggf.316326.xyz

TS:   path.extname("a.txt")
来源：http://bpn.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xuf.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dfr.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dqf.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bsk.dashuyun.cn

[F11] 复制与移动文件
来源：http://epn.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nen.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gst.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sip.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://msi.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bjo.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ond.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vor.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ovy.jyoumei.cn

[F12] CSV 读写
来源：http://sqk.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ciu.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pvk.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zca.fzhhl.top

TS:   // 同上
来源：http://abr.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ppi.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vxv.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://apx.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://imm.hammf.cn

================================================================================
来源：http://ldn.nanxinkj.top

G. 面向对象
来源：http://gsu.hfpthk.cn

================================================================================
来源：http://utz.ppjwa.cn

[G01] 定义类
来源：http://znw.nwbrower.top

Py:   class User: pass
来源：http://vju.hnqzz.top

PHP:  class User {}
来源：http://kge.epnwcf.com

JS:   class User {}
来源：http://qep.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://gor.hesvh.cn

Java: class User {}
来源：http://lmp.cdnleiting.top

Go:   type User struct { Name string }
来源：http://ttu.sweek.top

Ruby: class User; end
来源：http://dtq.hammf.cn

C#:   class User {}
来源：http://lyb.gzhubu.top

[G02] 构造函数
来源：http://hwq.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://hmt.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://jpi.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://scy.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://euw.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://ngc.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://crw.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://rrw.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://mqc.yanxiufei.cn

[G03] 实例属性
来源：http://qwe.9152youxi.cn

Py:   self.name = "x"
来源：http://pmi.tian-w.cn

PHP:  public string $name = "x";
来源：http://aod.xylfe.cn

JS:   this.name = "x";
来源：http://xec.yonumen.top

TS:   name: string = "x";
来源：http://tjs.vehdjk.com

Java: private String name;
来源：http://atu.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mjb.daria6918.cn

Ruby: @name = "x"
来源：http://lkv.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://iau.yuxming.cn

[G04] 定义方法
来源：http://hly.vehdjk.com

Py:   def greet(self): return self.name
来源：http://onv.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cwe.redwolf501.top

JS:   greet() { return this.name; }
来源：http://kfv.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://sky.snrcjt.cn

Java: String greet() { return name; }
来源：http://mro.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fvs.tanke756.top

Ruby: def greet; @name; end
来源：http://yqv.aizwys.cn

C#:   public string Greet() => Name;
来源：http://hwp.chenzaomai.com

[G05] 继承
来源：http://wre.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://hsn.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://twg.xuanzx.com

JS:   class Admin extends User {}
来源：http://gdb.fehbvm.com

TS:   class Admin extends User {}
来源：http://zvh.guowangkeji.top

Java: class Admin extends User {}
来源：http://nie.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://trb.shuidangran.top

Ruby: class Admin < User; end
来源：http://yat.jyoumei.cn

C#:   class Admin : User {}
来源：http://quv.tanke756.top

[G06] 重写方法
来源：http://bsb.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://ary.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://izm.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://xqr.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://qky.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://qef.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ndp.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://tag.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://qoe.hongshengwenyu.top

[G07] 调用父类方法
来源：http://hzo.shuidangran.top

Py:   super().greet()
来源：http://btx.cqqwz.cn

PHP:  parent::greet();
来源：http://vcn.nanxuanxn.top

JS:   super.greet();
来源：http://raw.sysykeji.top

TS:   super.greet();
来源：http://epp.epnwcf.com

Java: super.greet();
来源：http://gsn.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wbt.zhongyouzk.top

Ruby: super
来源：http://bmi.vehdjk.com

C#:   base.Greet();
来源：http://ulh.tanke756.top

[G08] 静态方法与属性
来源：http://hrj.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iso.redwolf501.top

PHP:  public static function f() {}
来源：http://ytr.xuetiantiany.cn

JS:   static f() {}
来源：http://aei.quarkkingdee.top

TS:   static f(): void {}
来源：http://uun.9152youxi.cn

Java: static void f() {}
来源：http://pzh.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://efl.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://sfk.redwolf501.top

C#:   public static void F() {}
来源：http://bah.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://bnc.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://obt.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://rco.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://obw.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://stt.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://kae.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://yde.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://exm.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://bpj.zhongyouzk.top

[G10] 访问控制
来源：http://dmv.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://jza.ehwqpu.com

PHP:  public / protected / private
来源：http://kzg.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://pcs.ivvv.top

TS:   public / protected / private
来源：http://eia.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://hzb.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kok.zhongyouzk.top

Ruby: public / protected / private
来源：http://xrk.tianlin.xyz

C#:   public / protected / private / internal
来源：http://frw.gaohongyu789.top

[G11] getter / setter
来源：http://iij.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://ehv.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rmq.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://ssi.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://cda.yongpay.top

Java: public String getName() { return name; }
来源：http://ile.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://slt.daxiang520.top

Ruby: attr_accessor :name
来源：http://vtr.fzhhl.top

C#:   public string Name { get; set; }
来源：http://lzs.xinyue.icu

[G12] 对象转字符串
来源：http://kgm.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://yky.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vev.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://qjq.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://ntv.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://uql.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://yls.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://hta.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://hvm.9152youxi.cn

[G13] 判断对象类型
来源：http://ldj.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://ayy.havefunace.top

PHP:  $u instanceof User
来源：http://jrg.sxryk.cn

JS:   u instanceof User
来源：http://blu.zhengqikj.top

TS:   u instanceof User
来源：http://rxs.xziqi.cn

Java: u instanceof User
来源：http://mjt.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fdr.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://tnd.havefunace.top

C#:   u is User
来源：http://aag.jyoumei.cn

[G14] 数据类 / record
来源：http://skv.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wib.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://oez.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://qhj.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://olv.yueranfly.top

Java: record User(String name, int age) {}
来源：http://txs.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://akp.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gzs.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://tgm.zhoulong.xyz

[G15] 枚举
来源：http://ksg.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zkr.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ikz.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://smx.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fat.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://jri.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hcu.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://uki.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://irw.yj202588.top

[G16] 对象转数组 / 字典
来源：http://hvt.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mgx.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://jpi.hysaishi.cn

JS:   Object.entries(obj)
来源：http://qfg.svipenyu.cn

TS:   Object.entries(obj)
来源：http://cge.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xdl.zhoulong.xyz


<!-- 参考信息 -->