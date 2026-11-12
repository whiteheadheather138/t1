代发 wailian999

Ruby: s.lines
来源：http://iqv.9152youxi.cn

C#:   s.Split('\n')
来源：http://zje.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://mjw.guowangkeji.top

Py:   if not s:
来源：http://wos.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbs.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hga.nanxinkj.top

TS:   if (s === "") {}
来源：http://vgq.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://jhw.vqdsnc.cn

Go:   if s == "" {}
来源：http://okb.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://vle.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gzz.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://mxj.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eaz.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qrb.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zfq.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yij.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ayx.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://kgr.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://esz.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bec.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://umc.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://len.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xcc.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqu.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hna.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fqd.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://twj.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://fbd.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rjs.xylfe.cn

================================================================================
来源：http://tyr.guannengcc.top

F. 文件与目录
来源：http://vhs.jinqigfzy.top

================================================================================
来源：http://hwf.haohaochexian.top

[F01] 读取整个文件
来源：http://ujm.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fhp.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://wyu.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zit.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sld.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bbt.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mvj.birdmap.top

Ruby: File.read("a.txt")
来源：http://cvl.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://cgb.aizwys.cn

[F02] 逐行读取文件
来源：http://igj.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yam.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xcb.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://khx.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpm.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vsp.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eio.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vtw.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://njc.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://zuq.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://idk.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cog.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jjh.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kvt.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://okk.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kcx.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://pgs.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fbv.zhixingplan.top

[F04] 追加写入文件
来源：http://mok.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fwx.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nkn.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ygl.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vyn.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ulb.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mci.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dub.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oqj.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://voq.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eyb.tarul.cn

PHP:  file_exists("a.txt");
来源：http://fzc.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://oyr.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://lqz.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://gth.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pdm.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://cly.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://fmy.wangdashe.top

[F06] 删除文件
来源：http://gbn.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://why.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://rfw.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://zqb.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://spj.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cqb.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://sid.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://zgz.wangdashe.top

C#:   File.Delete("a.txt");
来源：http://pss.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://ftw.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ojd.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wfz.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzr.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dkr.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vlj.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zge.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hfs.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vrm.shangyingyoupin.top

[F08] 遍历目录
来源：http://ard.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://hxx.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ijj.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://uwf.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://xva.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://knl.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://osh.birdmap.top

Ruby: Dir.children("dir")
来源：http://qpv.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://bqx.tian-w.cn

[F09] 获取文件大小
来源：http://nap.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://oup.fzhhl.top

PHP:  filesize("a.txt");
来源：http://uiz.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://bos.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://vqj.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uyp.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gwe.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://npa.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://rbc.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://fxk.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nff.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://apn.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eiy.tarul.cn

TS:   path.extname("a.txt")
来源：http://ost.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jqg.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vbl.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hmb.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://paq.yvedp.cn

[F11] 复制与移动文件
来源：http://qft.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://voo.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bzo.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mbl.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhc.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ftq.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xah.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lnw.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sju.zhengqikj.top

[F12] CSV 读写
来源：http://oqs.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ayz.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kae.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uet.jyoumei.cn

TS:   // 同上
来源：http://ljc.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dss.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xnq.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://znx.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://onw.smart0.xyz

================================================================================
来源：http://ysd.havefunace.top

G. 面向对象
来源：http://sch.jinyuanbaomall.cn

================================================================================
来源：http://ewx.yvedp.cn

[G01] 定义类
来源：http://iyo.bjfxy.top

Py:   class User: pass
来源：http://zft.daxiang520.top

PHP:  class User {}
来源：http://xsg.yueranfly.top

JS:   class User {}
来源：http://soj.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://dzn.zhengqikj.top

Java: class User {}
来源：http://nks.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://kgu.guannengcc.top

Ruby: class User; end
来源：http://yyt.jinqigufen.top

C#:   class User {}
来源：http://xgy.shuidangran.top

[G02] 构造函数
来源：http://dlm.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://aop.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://dms.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://jyq.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://xsy.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://bjp.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nkw.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://yrm.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://clv.fehbvm.com

[G03] 实例属性
来源：http://xuo.ehwqpu.com

Py:   self.name = "x"
来源：http://qpf.hywenlv.cn

PHP:  public string $name = "x";
来源：http://ozw.jianghu66.top

JS:   this.name = "x";
来源：http://lmr.gogol.net.cn

TS:   name: string = "x";
来源：http://aau.tianlin.xyz

Java: private String name;
来源：http://sji.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qzr.gogol.net.cn

Ruby: @name = "x"
来源：http://akv.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://uak.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://ucl.pycfn.com

Py:   def greet(self): return self.name
来源：http://usi.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jbt.zycfv.cn

JS:   greet() { return this.name; }
来源：http://jxb.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://gzg.nwbrower.top

Java: String greet() { return name; }
来源：http://kni.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://pbe.zdqjudy.top

Ruby: def greet; @name; end
来源：http://nib.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://pwl.jyoumei.cn

[G05] 继承
来源：http://giw.sysykeji.top

Py:   class Admin(User): pass
来源：http://hfw.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://qov.mhx1999.top

JS:   class Admin extends User {}
来源：http://bvj.hcnkem.com

TS:   class Admin extends User {}
来源：http://omr.mhx1999.top

Java: class Admin extends User {}
来源：http://wzz.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lve.ydzc1.top

Ruby: class Admin < User; end
来源：http://uxl.c1oappe.top

C#:   class Admin : User {}
来源：http://kwp.hfpthk.cn

[G06] 重写方法
来源：http://cld.tanke756.top

Py:   def greet(self): return "admin"
来源：http://cef.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nyl.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://kbf.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://nls.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://thi.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rma.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://gpx.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://cid.cqqwz.cn

[G07] 调用父类方法
来源：http://iqs.cucudq.cn

Py:   super().greet()
来源：http://qgr.aizwys.cn

PHP:  parent::greet();
来源：http://yai.smart0.xyz

JS:   super.greet();
来源：http://whk.52xcode.cn

TS:   super.greet();
来源：http://wwy.tianlin.xyz

Java: super.greet();
来源：http://ywd.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qib.xinyue.icu

Ruby: super
来源：http://ohg.9152youxi.cn

C#:   base.Greet();
来源：http://ipq.tanke756.top

[G08] 静态方法与属性
来源：http://xyo.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vvg.guowangkeji.top

PHP:  public static function f() {}
来源：http://lwf.uphjek.com

JS:   static f() {}
来源：http://rmj.redwolf501.top

TS:   static f(): void {}
来源：http://lxo.yuanzhike.top

Java: static void f() {}
来源：http://vph.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://msq.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://tei.haohaochexian.top

C#:   public static void F() {}
来源：http://cin.hnqzz.top

[G09] 接口 / 抽象类
来源：http://jeo.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://dqm.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://mso.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ouj.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://lva.yvedp.cn

Java: interface Shape { double area(); }
来源：http://rqc.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://ehv.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://haf.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://wmw.shanyushiyangkeji.top

[G10] 访问控制
来源：http://phn.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://vpm.feifeiyinyue.top

PHP:  public / protected / private
来源：http://cko.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://kwz.nanxinkj.top

TS:   public / protected / private
来源：http://whl.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://xqk.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rjf.yj20258.top

Ruby: public / protected / private
来源：http://ekz.fengsongda.top

C#:   public / protected / private / internal
来源：http://avl.meibo888.top

[G11] getter / setter
来源：http://wzd.ivvv.top

Py:   @property 与 @x.setter
来源：http://bfq.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bof.bjfxy.top

JS:   get name() { return this._name; }
来源：http://bkv.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://sxh.0kj1m.cn

Java: public String getName() { return name; }
来源：http://zss.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tdn.yj202588.top

Ruby: attr_accessor :name
来源：http://eck.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://rwr.yueranfly.top

[G12] 对象转字符串
来源：http://azw.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://hwj.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jet.yongpay.top

JS:   toString() { return this.name; }
来源：http://awa.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://dpm.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://dgw.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://iqv.smart0.xyz

Ruby: def to_s; @name; end
来源：http://swo.316326.xyz

C#:   public override string ToString() => Name;
来源：http://ygk.yueranfly.top

[G13] 判断对象类型
来源：http://tcw.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://ynz.jinqigfzy.top

PHP:  $u instanceof User
来源：http://ecz.hammf.cn

JS:   u instanceof User
来源：http://bmj.nwbrower.top

TS:   u instanceof User
来源：http://jqk.xylfe.cn

Java: u instanceof User
来源：http://lao.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cwm.bjfxy.top

Ruby: u.is_a?(User)
来源：http://out.quarkkingdee.top

C#:   u is User
来源：http://oyf.meibo888.top

[G14] 数据类 / record
来源：http://fix.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://llx.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://npg.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://evw.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://ocf.havefunace.top

Java: record User(String name, int age) {}
来源：http://rjp.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://yoe.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ezp.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://aed.fanxiaobao.xyz

[G15] 枚举
来源：http://rwv.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fzg.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bhy.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fhf.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ztm.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://qjm.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yxj.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://gvl.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://amf.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://ajh.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbj.yj202588.top

PHP:  get_object_vars($obj);
来源：http://rak.snrcjt.cn

JS:   Object.entries(obj)
来源：http://cbl.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://pro.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://isn.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fqc.tarul.cn

Ruby: obj.instance_variables
来源：http://oct.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://yqu.yj202588.top

================================================================================
来源：http://men.wangdashe.top

H. 异常与错误处理
来源：http://nom.jqgfzy.top

================================================================================
来源：http://nlw.0kj1m.cn

[H01] try / catch 基础
来源：http://quh.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://swd.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whu.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://trd.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pwc.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gke.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iob.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://njr.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://inz.xinyue.icu

[H02] finally / ensure 收尾
来源：http://smt.chenlongwang.top


<!-- 参考信息 -->