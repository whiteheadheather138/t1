代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://wsk.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aqb.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dji.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ziu.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tmu.jianghu66.top

[E19] 多行文本按行拆分
来源：http://aaf.jianghu66.top

Py:   s.splitlines()
来源：http://jil.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ceh.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://mhl.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://cyy.ivvv.top

Java: s.lines().toList()
来源：http://jlk.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://hlj.gogol.net.cn

Ruby: s.lines
来源：http://pjm.gaohongyu789.top

C#:   s.Split('\n')
来源：http://zvi.daxiang520.top

[E20] 判断字符串是否为空
来源：http://xfp.jqgufenzy.top

Py:   if not s:
来源：http://tnc.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mjo.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nmx.316326.xyz

TS:   if (s === "") {}
来源：http://roo.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://xwz.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://cfd.hammf.cn

Ruby: if s.empty?
来源：http://zsz.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rdy.ctjpmb.com

[E21] 超长截断加省略号
来源：http://mna.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rrz.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pzd.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sik.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwq.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fka.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://kpa.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jjg.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcs.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://bwr.sufxvd.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dvm.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baf.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wee.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hdb.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fut.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://opm.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://aal.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wyw.sufxvd.cn

================================================================================
来源：http://wip.tanke756.top

F. 文件与目录
来源：http://bgd.jlsjyb.cn

================================================================================
来源：http://dlb.sxryk.cn

[F01] 读取整个文件
来源：http://wzi.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rbk.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://yan.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wql.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://upa.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xru.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sfq.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://bjz.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xwi.c1oappe.top

[F02] 逐行读取文件
来源：http://lkb.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tmj.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://saf.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vem.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://csj.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dzj.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xie.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hmn.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baj.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://zyc.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fyf.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bva.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ouh.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://naz.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yqg.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dvv.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://pkb.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mdc.hesvh.cn

[F04] 追加写入文件
来源：http://zhe.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lzw.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sqx.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kol.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fpx.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://twr.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://swn.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://phc.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mqg.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://dxy.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vys.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://zqm.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://poc.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://any.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bdh.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uge.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://dtw.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://tmb.bjfxy.top

[F06] 删除文件
来源：http://lrh.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://zrp.hammf.cn

PHP:  unlink("a.txt");
来源：http://tcy.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://fni.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://cty.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xmt.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://qbo.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://dko.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://osv.mhx1999.top

[F07] 创建目录（含多级）
来源：http://yzy.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fin.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vbb.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hqw.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kaa.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hrj.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://epn.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ecr.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ztx.9152youxi.cn

[F08] 遍历目录
来源：http://qwb.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://jdn.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ebw.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://fch.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://img.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dgm.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lls.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://cnl.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://icy.cqqwz.cn

[F09] 获取文件大小
来源：http://lim.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://hbh.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://gqq.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://ymr.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://pew.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qnz.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vup.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://msa.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://iay.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://vek.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mog.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mdq.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rji.smart0.xyz

TS:   path.extname("a.txt")
来源：http://xyq.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wdw.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://trd.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qem.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xcs.xinyue.icu

[F11] 复制与移动文件
来源：http://qsx.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bcg.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nxg.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eyp.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://djy.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cdl.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://awg.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cas.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xhd.jlsjyb.cn

[F12] CSV 读写
来源：http://qfz.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eyj.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://axd.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qkh.fehbvm.com

TS:   // 同上
来源：http://ozz.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mtp.cashguo.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xno.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xyt.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://anf.yvedp.cn

================================================================================
来源：http://rqv.cashguo.top

G. 面向对象
来源：http://gok.zdbjq.cn

================================================================================
来源：http://oxo.wangshuangyany.cn

[G01] 定义类
来源：http://wbl.yfazqb.com

Py:   class User: pass
来源：http://tge.quarkkingdee.top

PHP:  class User {}
来源：http://wis.yvedp.cn

JS:   class User {}
来源：http://uuf.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://eyy.feifeiyinyue.top

Java: class User {}
来源：http://iwf.xuanzx.com

Go:   type User struct { Name string }
来源：http://tgw.sysykeji.top

Ruby: class User; end
来源：http://zcq.sjlbkw.cn

C#:   class User {}
来源：http://lqu.tanke756.top

[G02] 构造函数
来源：http://hsh.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://fbj.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://ods.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://bfj.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://fay.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://hel.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uhh.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://frd.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://zsy.yvedp.cn

[G03] 实例属性
来源：http://vbx.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://zwr.yuanzhike.top

PHP:  public string $name = "x";
来源：http://ykr.fktsv.cn

JS:   this.name = "x";
来源：http://cbq.smart0.xyz

TS:   name: string = "x";
来源：http://fug.shuidangran.top

Java: private String name;
来源：http://plg.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oos.aibaodan.cn

Ruby: @name = "x"
来源：http://bxr.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://atv.jqgufenzy.top

[G04] 定义方法
来源：http://tuv.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://dfa.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://chf.yj20258.top

JS:   greet() { return this.name; }
来源：http://iiw.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://tob.vehdjk.com

Java: String greet() { return name; }
来源：http://dnx.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://efi.ydzc1.top

Ruby: def greet; @name; end
来源：http://pyp.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://gil.sweek.top

[G05] 继承
来源：http://ubx.hcnkem.com

Py:   class Admin(User): pass
来源：http://xci.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://qrn.zdqjudy.top

JS:   class Admin extends User {}
来源：http://hhy.haohaochexian.top

TS:   class Admin extends User {}
来源：http://omb.zdqjudy.top

Java: class Admin extends User {}
来源：http://xkd.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://epc.fehbvm.com

Ruby: class Admin < User; end
来源：http://pir.ybcxt.top

C#:   class Admin : User {}
来源：http://ewh.pycfn.com

[G06] 重写方法
来源：http://fij.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://aes.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sqr.cheryme.top

JS:   greet() { return "admin"; }
来源：http://rzo.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://gpg.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://mso.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lru.cashguo.top

Ruby: def greet; "admin"; end
来源：http://tfq.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://dho.daria6918.cn

[G07] 调用父类方法
来源：http://tyq.xuetiantiany.cn

Py:   super().greet()
来源：http://xkk.sufxvd.cn

PHP:  parent::greet();
来源：http://kfz.aizwys.cn

JS:   super.greet();
来源：http://sln.mhx1999.top

TS:   super.greet();
来源：http://xeb.jinyuanbaomall.cn

Java: super.greet();
来源：http://ygs.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://htv.sxryk.cn

Ruby: super
来源：http://hpo.tanke756.top

C#:   base.Greet();
来源：http://hbu.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://pqd.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jiq.snrcjt.cn

PHP:  public static function f() {}
来源：http://add.dianchejie.cn

JS:   static f() {}
来源：http://jzq.xylfe.cn

TS:   static f(): void {}
来源：http://jfs.cqqwz.cn

Java: static void f() {}
来源：http://lcv.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jud.smart0.xyz

Ruby: def self.f; end
来源：http://cep.aizwys.cn

C#:   public static void F() {}
来源：http://pnd.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://xbo.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://ijz.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://vcz.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ggh.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://ztg.tarul.cn

Java: interface Shape { double area(); }
来源：http://lrc.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://qvp.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vlc.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://bhy.kuanghao11.cn

[G10] 访问控制
来源：http://tpm.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://fkh.redwolf501.top

PHP:  public / protected / private
来源：http://xag.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://cgt.52xcode.cn

TS:   public / protected / private
来源：http://qwz.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://sjj.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mmy.shangyingyoupin.top

Ruby: public / protected / private
来源：http://fgo.sxryk.cn

C#:   public / protected / private / internal
来源：http://gze.cucudq.cn

[G11] getter / setter
来源：http://yrk.pycfn.com

Py:   @property 与 @x.setter
来源：http://pvk.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rjh.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://imt.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://kos.316326.xyz

Java: public String getName() { return name; }
来源：http://uaz.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rkn.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://hxx.havefunace.top

C#:   public string Name { get; set; }
来源：http://fvl.zycfv.cn

[G12] 对象转字符串
来源：http://moc.ivvv.top

Py:   def __str__(self): return self.name
来源：http://nwe.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://atr.cucudq.cn

JS:   toString() { return this.name; }
来源：http://gtc.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://jmh.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://bpw.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://xdz.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://mdf.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://tal.tarul.cn

[G13] 判断对象类型
来源：http://kwt.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://rrc.havefunace.top

PHP:  $u instanceof User
来源：http://ygc.zdqjudy.top

JS:   u instanceof User
来源：http://qhn.tianlin.xyz

TS:   u instanceof User
来源：http://are.dianchejie.cn

Java: u instanceof User
来源：http://qfa.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nqz.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://opg.cdnleiting.top

C#:   u is User
来源：http://boc.cashguo.top

[G14] 数据类 / record
来源：http://fte.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tgq.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://iqn.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://avd.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://rni.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://exv.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://kak.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mhl.hammf.cn

C#:   record User(string Name, int Age);
来源：http://uag.gzhubu.top

[G15] 枚举
来源：http://sow.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hip.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lff.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ifs.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zoi.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://gnu.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cna.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://deo.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sis.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://sdj.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ybh.sweek.top

PHP:  get_object_vars($obj);
来源：http://gxi.jianghu66.top

JS:   Object.entries(obj)
来源：http://cfz.yuanzhike.top

TS:   Object.entries(obj)
来源：http://jgf.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pvc.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://dbl.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://tzl.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://hie.ppjwa.cn

================================================================================
来源：http://ilq.pycfn.com


<!-- 参考信息 -->