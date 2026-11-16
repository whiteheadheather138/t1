代发 wailian999

[E18] 模板占位符替换
来源：http://ozg.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kln.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://enj.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://pep.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hhw.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ign.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mdw.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qji.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://brd.sxryk.cn

[E19] 多行文本按行拆分
来源：http://zbl.shzxlz.cn

Py:   s.splitlines()
来源：http://qab.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pur.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://eei.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://fzx.52xcode.cn

Java: s.lines().toList()
来源：http://tim.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://mdl.hnxiangtu.top

Ruby: s.lines
来源：http://xsc.jiagoushi.top

C#:   s.Split('\n')
来源：http://ayo.fehbvm.com

[E20] 判断字符串是否为空
来源：http://dqr.jlsjyb.cn

Py:   if not s:
来源：http://zuc.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kas.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://txj.zhengqikj.top

TS:   if (s === "") {}
来源：http://qnr.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://pkz.pengpengdd.cyou

Go:   if s == "" {}
来源：http://plx.daria6918.cn

Ruby: if s.empty?
来源：http://eop.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pnw.jinqigufen.top

[E21] 超长截断加省略号
来源：http://txw.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yxu.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xiz.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hgt.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cyt.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yto.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://rdg.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kcy.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fkw.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://rvb.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zbf.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://igv.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzi.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://byb.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ahd.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://msf.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://pwa.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cjr.hnqzz.top

================================================================================
来源：http://zgc.zhixingplan.top

F. 文件与目录
来源：http://dbd.zhijiandao.cn

================================================================================
来源：http://duw.meibo888.top

[F01] 读取整个文件
来源：http://jhp.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uwk.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://syb.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gsb.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pub.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qps.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dem.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://gkj.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://yna.xuanzx.com

[F02] 逐行读取文件
来源：http://wdn.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fqd.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ogq.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://djc.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zks.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zjq.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xjj.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bfn.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://erz.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://neo.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qzz.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggy.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfo.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ths.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://znt.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eur.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://uoe.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kho.yonumen.top

[F04] 追加写入文件
来源：http://slp.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pov.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wza.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijs.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pia.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wqg.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qph.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hsi.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cqh.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://igd.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rxw.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://hef.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://erf.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://ixr.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mby.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dxd.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://hdl.birdmap.top

C#:   File.Exists("a.txt")
来源：http://zob.daria6918.cn

[F06] 删除文件
来源：http://dxu.cucudq.cn

Py:   os.remove("a.txt")
来源：http://kfr.tian-w.cn

PHP:  unlink("a.txt");
来源：http://bfk.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qgk.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://eoi.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gyo.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://rtu.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://iji.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://rpw.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://xqp.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kde.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cup.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nui.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jbb.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iwd.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://obq.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tcj.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tsj.jinghuilouyu.cn

[F08] 遍历目录
来源：http://vej.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://qmk.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bup.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://bun.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://kfx.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lta.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rwj.aizwys.cn

Ruby: Dir.children("dir")
来源：http://jzq.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://siy.ivvv.top

[F09] 获取文件大小
来源：http://djw.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://dna.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://xqe.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://qce.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://ymw.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://pra.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://erd.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://lpu.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://yga.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://bnc.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xfu.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ylv.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rld.cucudq.cn

TS:   path.extname("a.txt")
来源：http://vpe.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ksz.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://puv.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fju.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wef.yueranfly.top

[F11] 复制与移动文件
来源：http://dta.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xrk.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zak.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rbd.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yin.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ylz.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://axw.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aof.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nzu.uphjek.com

[F12] CSV 读写
来源：http://csb.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://snl.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eni.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nrs.zhiwuduotai.top

TS:   // 同上
来源：http://cnr.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kxv.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://htq.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://coj.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ubp.chenzaomai.com

================================================================================
来源：http://zpt.svipenyu.cn

G. 面向对象
来源：http://com.jianghu66.top

================================================================================
来源：http://pql.xziqi.cn

[G01] 定义类
来源：http://hsy.zycfv.cn

Py:   class User: pass
来源：http://lob.nwbrower.top

PHP:  class User {}
来源：http://jta.bbcook.cn

JS:   class User {}
来源：http://reg.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://qpn.wangshuangyany.cn

Java: class User {}
来源：http://hoc.zycfv.cn

Go:   type User struct { Name string }
来源：http://nmf.zhaomingkeji.xyz

Ruby: class User; end
来源：http://qsl.yj202588.top

C#:   class User {}
来源：http://dzq.jinghuilouyu.cn

[G02] 构造函数
来源：http://xov.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://kuo.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://typ.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://upd.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://zme.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://opz.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hcy.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://qrr.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://mph.yj20258888.top

[G03] 实例属性
来源：http://mbz.zhoulong.xyz

Py:   self.name = "x"
来源：http://por.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://znn.havefunace.top

JS:   this.name = "x";
来源：http://vcw.yuanzhike.top

TS:   name: string = "x";
来源：http://jpe.cqqwz.cn

Java: private String name;
来源：http://lmn.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nib.yvedp.cn

Ruby: @name = "x"
来源：http://dfy.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://isx.9152youxi.cn

[G04] 定义方法
来源：http://vgl.316326.xyz

Py:   def greet(self): return self.name
来源：http://zst.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aaj.zhixingplan.top

JS:   greet() { return this.name; }
来源：http://qdu.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://ntc.aibaodan.cn

Java: String greet() { return name; }
来源：http://vae.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lvv.yvedp.cn

Ruby: def greet; @name; end
来源：http://kwi.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://eyo.zhixingplan.top

[G05] 继承
来源：http://yio.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://phv.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://kmy.ivvv.top

JS:   class Admin extends User {}
来源：http://bgq.hcnkem.com

TS:   class Admin extends User {}
来源：http://xbt.chenzaomai.com

Java: class Admin extends User {}
来源：http://tjy.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pdu.wangdashe.top

Ruby: class Admin < User; end
来源：http://fpz.jinqigufen.top

C#:   class Admin : User {}
来源：http://kww.cheryme.top

[G06] 重写方法
来源：http://kon.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://rxo.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hdw.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://eff.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://ecp.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://plj.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://snr.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://ubr.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://nwx.ppjwa.cn

[G07] 调用父类方法
来源：http://koy.ctjpmb.com

Py:   super().greet()
来源：http://rhh.yj202588.top

PHP:  parent::greet();
来源：http://hrb.ybcxt.top

JS:   super.greet();
来源：http://nks.chenlongwang.top

TS:   super.greet();
来源：http://mwz.yj20258.top

Java: super.greet();
来源：http://ljr.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ozx.haohaochexian.top

Ruby: super
来源：http://rit.yvedp.cn

C#:   base.Greet();
来源：http://uvy.dashuyun.cn

[G08] 静态方法与属性
来源：http://jmb.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://axd.sjlbkw.cn

PHP:  public static function f() {}
来源：http://trb.iojbl.cn

JS:   static f() {}
来源：http://eni.ppjwa.cn

TS:   static f(): void {}
来源：http://ivd.zdqjudy.top

Java: static void f() {}
来源：http://chj.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hbo.nwbrower.top

Ruby: def self.f; end
来源：http://rof.hnqzz.top

C#:   public static void F() {}
来源：http://xgv.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://upu.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://dqo.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://ahi.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oww.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://uad.guannengcc.top

Java: interface Shape { double area(); }
来源：http://scq.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://vyn.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pag.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://fmv.nanxuanxn.top

[G10] 访问控制
来源：http://bdn.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://cqf.meibo888.top

PHP:  public / protected / private
来源：http://qaj.yvedp.cn

JS:   #private 字段；其余公开
来源：http://bbx.tianlin.xyz

TS:   public / protected / private
来源：http://lms.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://mlk.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ava.yanxiufei.cn

Ruby: public / protected / private
来源：http://byy.yvedp.cn

C#:   public / protected / private / internal
来源：http://qin.haohaochexian.top

[G11] getter / setter
来源：http://abn.daria6918.cn

Py:   @property 与 @x.setter
来源：http://bqg.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nvv.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://gsc.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://ffq.epnwcf.com

Java: public String getName() { return name; }
来源：http://xhg.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rhb.shuidangran.top

Ruby: attr_accessor :name
来源：http://rgg.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://kes.dashuyun.cn

[G12] 对象转字符串
来源：http://yzz.sweek.top

Py:   def __str__(self): return self.name
来源：http://ghq.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zvv.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://xmn.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://qse.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://pim.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://usm.fehbvm.com

Ruby: def to_s; @name; end
来源：http://qil.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://try.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://kmd.zycfv.cn

Py:   isinstance(u, User)
来源：http://ier.quarkkingdee.top

PHP:  $u instanceof User
来源：http://xjh.shanyushiyangtech.top

JS:   u instanceof User
来源：http://qmo.kuanghao11.cn

TS:   u instanceof User
来源：http://khh.zhaomingkeji.xyz

Java: u instanceof User
来源：http://tan.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pey.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://alm.fktsv.cn

C#:   u is User
来源：http://bwv.smart0.xyz

[G14] 数据类 / record
来源：http://cqt.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xqs.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://lab.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://apw.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://ayb.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://djq.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://llo.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ens.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://jvc.shzxlz.cn

[G15] 枚举
来源：http://yed.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ssj.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cvu.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ypc.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dpd.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://krm.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fax.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://asw.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mfz.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://lan.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wte.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://zds.yonumen.top

JS:   Object.entries(obj)
来源：http://qua.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://cxu.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://unw.tianlin.xyz


<!-- 参考信息 -->