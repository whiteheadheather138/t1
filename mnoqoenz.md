代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gnk.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzu.hfpthk.cn

Ruby: s.capitalize
来源：http://kex.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nvl.andypj.xyz

[E18] 模板占位符替换
来源：http://eql.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rky.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jkp.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fcj.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jgb.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ner.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://prr.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nzn.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qrk.yj20258.top

[E19] 多行文本按行拆分
来源：http://uxe.fehbvm.com

Py:   s.splitlines()
来源：http://xau.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vgl.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://owc.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://idx.xuanzx.com

Java: s.lines().toList()
来源：http://ekp.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://wax.zdqjudy.top

Ruby: s.lines
来源：http://iqt.cqqwz.cn

C#:   s.Split('\n')
来源：http://upi.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://yhu.birdmap.top

Py:   if not s:
来源：http://uta.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sra.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zxf.daxiang520.top

TS:   if (s === "") {}
来源：http://cqg.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://tty.xinyue.icu

Go:   if s == "" {}
来源：http://egj.shangyingyoupin.top

Ruby: if s.empty?
来源：http://rwd.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pst.sweek.top

[E21] 超长截断加省略号
来源：http://bpq.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://his.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://awz.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uzh.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rei.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://izl.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://klk.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://okq.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oqn.hnqzz.top

[E22] 字节长度与字符长度
来源：http://klz.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xxb.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nvs.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hlk.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekk.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rhs.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ejp.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://qso.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tjb.ydzc1.top

================================================================================
来源：http://fwn.yanxiufei.cn

F. 文件与目录
来源：http://qtp.yueranfly.top

================================================================================
来源：http://hgb.xziqi.cn

[F01] 读取整个文件
来源：http://emb.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cyr.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://wfw.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dxy.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dhj.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://etw.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ing.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://dxy.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://wrk.cqqwz.cn

[F02] 逐行读取文件
来源：http://xho.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://emd.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rza.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxb.hfpthk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xey.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qph.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zoq.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nci.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://txf.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://pri.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yud.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggf.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrz.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ukd.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zea.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://chs.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://hoh.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tjr.52xcode.cn

[F04] 追加写入文件
来源：http://zmm.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kev.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hxp.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tvs.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipd.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fkv.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tzn.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mha.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://juh.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://urw.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sco.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://wdo.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://klq.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://uil.zhoulong.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://axg.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://npa.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://xex.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://uko.feifeiyinyue.top

[F06] 删除文件
来源：http://fpj.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://vwm.ivvv.top

PHP:  unlink("a.txt");
来源：http://nes.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://nmv.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://fnw.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eki.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://azr.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://tmy.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://goi.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://dam.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oin.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hwq.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lmq.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fgf.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://czt.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oac.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bqe.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nuo.meibo888.top

[F08] 遍历目录
来源：http://rak.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://msk.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qwb.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://vzh.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://cil.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kcf.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qyf.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://dpy.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://zif.uphjek.com

[F09] 获取文件大小
来源：http://xqn.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://jzy.meibo888.top

PHP:  filesize("a.txt");
来源：http://agc.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://apd.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://kug.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://hbz.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bfs.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://sej.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://daj.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://tyk.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pmb.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vyr.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zjl.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://kvp.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nia.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yke.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ioo.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zje.daria6918.cn

[F11] 复制与移动文件
来源：http://nkw.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://shg.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pqx.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpt.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arm.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zyk.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ccf.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vkc.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://roq.xziqi.cn

[F12] CSV 读写
来源：http://xmg.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lkq.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lbx.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qbo.hnxiangtu.top

TS:   // 同上
来源：http://vcr.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://doq.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vbn.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bzs.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ndp.sufxvd.cn

================================================================================
来源：http://bhx.ivvv.top

G. 面向对象
来源：http://hla.aibaodan.cn

================================================================================
来源：http://gzu.gogol.net.cn

[G01] 定义类
来源：http://vwb.cdnleiting.top

Py:   class User: pass
来源：http://vpm.chenjidiqi.icu

PHP:  class User {}
来源：http://vyp.ehwqpu.com

JS:   class User {}
来源：http://izk.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://ugy.jinqigfzy.top

Java: class User {}
来源：http://rzf.xylfe.cn

Go:   type User struct { Name string }
来源：http://enh.fktsv.cn

Ruby: class User; end
来源：http://csh.wangshuangyany.cn

C#:   class User {}
来源：http://xay.hfpthk.cn

[G02] 构造函数
来源：http://tjv.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://dha.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ikq.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://kkd.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://fku.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://jbm.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bky.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://mum.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://jjd.hysaishi.cn

[G03] 实例属性
来源：http://egx.fktsv.cn

Py:   self.name = "x"
来源：http://jqx.iojbl.cn

PHP:  public string $name = "x";
来源：http://vjg.yueranfly.top

JS:   this.name = "x";
来源：http://mfn.snrcjt.cn

TS:   name: string = "x";
来源：http://rsx.zycfv.cn

Java: private String name;
来源：http://zjh.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zvr.yongpay.top

Ruby: @name = "x"
来源：http://vos.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://lha.hfpthk.cn

[G04] 定义方法
来源：http://aaw.52xcode.cn

Py:   def greet(self): return self.name
来源：http://ivf.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ccd.uphjek.com

JS:   greet() { return this.name; }
来源：http://gex.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://rlh.guowangkeji.top

Java: String greet() { return name; }
来源：http://dxu.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqu.zycfv.cn

Ruby: def greet; @name; end
来源：http://exj.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://sha.fktsv.cn

[G05] 继承
来源：http://jrp.ehwqpu.com

Py:   class Admin(User): pass
来源：http://wtb.havefunace.top

PHP:  class Admin extends User {}
来源：http://aky.jinqigufen.top

JS:   class Admin extends User {}
来源：http://okq.yj202588.top

TS:   class Admin extends User {}
来源：http://mly.cashguo.top

Java: class Admin extends User {}
来源：http://pxa.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kxa.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://wuz.meibo888.top

C#:   class Admin : User {}
来源：http://fpt.sweek.top

[G06] 重写方法
来源：http://ist.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://fcu.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wmx.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://miu.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://ikn.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://lkw.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dxo.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://sjq.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://qeo.zhixingplan.top

[G07] 调用父类方法
来源：http://poa.yangfankeji.com

Py:   super().greet()
来源：http://ffz.snrcjt.cn

PHP:  parent::greet();
来源：http://hey.hywenlv.cn

JS:   super.greet();
来源：http://xyu.svipenyu.cn

TS:   super.greet();
来源：http://ulk.yuanzhike.top

Java: super.greet();
来源：http://xqm.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://enq.0kj1m.cn

Ruby: super
来源：http://awg.316326.xyz

C#:   base.Greet();
来源：http://axl.zhongyouzk.top

[G08] 静态方法与属性
来源：http://atd.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hxp.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://yfk.ydzc1.top

JS:   static f() {}
来源：http://fpx.hongshengwenyu.top

TS:   static f(): void {}
来源：http://tdw.svipenyu.cn

Java: static void f() {}
来源：http://sug.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://foa.zdbjq.cn

Ruby: def self.f; end
来源：http://vaq.ydjk.org.cn

C#:   public static void F() {}
来源：http://ivr.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://bun.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://fhu.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qbg.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vhn.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://osy.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://nsl.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://vws.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ngu.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://mms.yuxming.cn

[G10] 访问控制
来源：http://rwz.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://nrz.ybcxt.top

PHP:  public / protected / private
来源：http://yei.yuxming.cn

JS:   #private 字段；其余公开
来源：http://uzu.hesvh.cn

TS:   public / protected / private
来源：http://qdm.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://emo.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dqe.kuanghao11.cn

Ruby: public / protected / private
来源：http://mmm.hcnkem.com

C#:   public / protected / private / internal
来源：http://vni.hnqzz.top

[G11] getter / setter
来源：http://zkh.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://cma.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pha.xinyue.icu

JS:   get name() { return this._name; }
来源：http://teb.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://rga.sysykeji.top

Java: public String getName() { return name; }
来源：http://jay.redwolf501.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://amt.ehwqpu.com

Ruby: attr_accessor :name
来源：http://fto.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://ejf.chenlongwang.top

[G12] 对象转字符串
来源：http://srp.yongpay.top

Py:   def __str__(self): return self.name
来源：http://zfo.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rby.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://jsv.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://mjm.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://pvu.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ozl.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://shd.cashguo.top

C#:   public override string ToString() => Name;
来源：http://eae.havefunace.top

[G13] 判断对象类型
来源：http://ubl.nwbrower.top

Py:   isinstance(u, User)
来源：http://dcb.hnqzz.top

PHP:  $u instanceof User
来源：http://int.cucudq.cn

JS:   u instanceof User
来源：http://dba.cheryme.top

TS:   u instanceof User
来源：http://con.meibo888.top

Java: u instanceof User
来源：http://env.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wvs.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://prp.jinqigufen.top

C#:   u is User
来源：http://ydj.hcnkem.com

[G14] 数据类 / record
来源：http://yds.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vgp.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://fvd.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://pya.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://wdl.guannengcc.top

Java: record User(String name, int age) {}
来源：http://cil.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://jlo.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qqq.cashguo.top

C#:   record User(string Name, int Age);
来源：http://vxh.ppjwa.cn

[G15] 枚举
来源：http://iwn.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lce.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rff.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://atz.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jnq.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://art.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dmn.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://nyo.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wkl.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://jea.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vlr.ctjpmb.com


<!-- 参考信息 -->