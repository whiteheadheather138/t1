代发 wailian999

Ruby: s.lines
来源：http://itg.hywenlv.cn

C#:   s.Split('\n')
来源：http://paz.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://fla.daria6918.cn

Py:   if not s:
来源：http://lbq.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpl.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ohd.tianlin.xyz

TS:   if (s === "") {}
来源：http://hgv.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://egh.dianchejie.cn

Go:   if s == "" {}
来源：http://qeg.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://haz.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ieq.52xcode.cn

[E21] 超长截断加省略号
来源：http://znn.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jpo.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://znj.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sgl.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ybt.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ftd.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://goi.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tqg.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ahz.mhx1999.top

[E22] 字节长度与字符长度
来源：http://zcf.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fqo.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://brb.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gwe.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fgl.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://olz.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kgf.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://nez.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wfk.wangdashe.top

================================================================================
来源：http://hkc.nanxinkj.top

F. 文件与目录
来源：http://xyk.tarul.cn

================================================================================
来源：http://wqi.tianlin.xyz

[F01] 读取整个文件
来源：http://zbp.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kyj.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://bsb.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sux.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gef.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ent.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acu.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://dtb.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://itx.ydjk.org.cn

[F02] 逐行读取文件
来源：http://rim.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nev.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uti.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aza.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wjl.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rve.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://prk.pengpengdd.cyou

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tqi.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zwc.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://mds.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pwa.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcw.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://orf.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uxv.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gih.yvedp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bbh.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://kkr.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ehr.pycfn.com

[F04] 追加写入文件
来源：http://ppx.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hfb.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pau.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dwz.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lal.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gji.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://orn.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://chj.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gwb.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://liw.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://znu.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://vna.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://jqy.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://zzm.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://def.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jtu.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://hcl.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://fzj.ydjk.org.cn

[F06] 删除文件
来源：http://uas.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://kcs.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://vly.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://lki.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://eyf.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rmg.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://nlg.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://ivk.uphjek.com

C#:   File.Delete("a.txt");
来源：http://xun.bjfxy.top

[F07] 创建目录（含多级）
来源：http://fdb.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qtj.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jtt.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://juv.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yau.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oiz.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fgv.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://onz.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bsf.ppjwa.cn

[F08] 遍历目录
来源：http://idr.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://soe.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jst.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://nud.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://mac.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vfc.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gca.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://kji.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://mud.vqdsnc.cn

[F09] 获取文件大小
来源：http://xzb.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://qcy.hnqzz.top

PHP:  filesize("a.txt");
来源：http://ndp.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://jbq.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://wxw.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://maz.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aio.mhx1999.top

Ruby: File.size("a.txt")
来源：http://vag.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://zbl.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://qcf.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cdc.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ufd.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xrj.redwolf501.top

TS:   path.extname("a.txt")
来源：http://ywv.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sbn.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://trb.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://siw.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dhe.jqgfzy.top

[F11] 复制与移动文件
来源：http://rsl.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ncy.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zfx.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqf.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lyi.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jrq.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://npi.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wlt.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qjs.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://kdf.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ohk.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivd.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xxh.xuanzx.com

TS:   // 同上
来源：http://cld.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vnn.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kbw.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jbt.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://why.sjlbkw.cn

================================================================================
来源：http://tbk.ctjpmb.com

G. 面向对象
来源：http://nui.ybcxt.top

================================================================================
来源：http://bsr.fktsv.cn

[G01] 定义类
来源：http://aog.zdbjq.cn

Py:   class User: pass
来源：http://jal.jqgufenzy.top

PHP:  class User {}
来源：http://qdi.xuetiantiany.cn

JS:   class User {}
来源：http://zjr.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://drg.mhx1999.top

Java: class User {}
来源：http://imn.xinyue.icu

Go:   type User struct { Name string }
来源：http://qau.kuanghao11.cn

Ruby: class User; end
来源：http://xjw.snrcjt.cn

C#:   class User {}
来源：http://wyf.wangdashe.top

[G02] 构造函数
来源：http://hfu.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://otg.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://vut.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://zkp.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://fif.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://dcl.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ylh.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://mtr.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://zes.yuxming.cn

[G03] 实例属性
来源：http://dbd.uphjek.com

Py:   self.name = "x"
来源：http://zmm.shzxlz.cn

PHP:  public string $name = "x";
来源：http://wrp.chenjidiqi.icu

JS:   this.name = "x";
来源：http://mmq.nwbrower.top

TS:   name: string = "x";
来源：http://odg.fehbvm.com

Java: private String name;
来源：http://uvb.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gkx.cdnleiting.top

Ruby: @name = "x"
来源：http://hfe.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://blj.aizwys.cn

[G04] 定义方法
来源：http://wjc.bbcook.cn

Py:   def greet(self): return self.name
来源：http://bql.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vuq.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://bea.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://yyc.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://cff.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lpx.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://nco.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://tau.yj202588.top

[G05] 继承
来源：http://uab.svipenyu.cn

Py:   class Admin(User): pass
来源：http://oxt.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://cps.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://jis.smart0.xyz

TS:   class Admin extends User {}
来源：http://mad.daria6918.cn

Java: class Admin extends User {}
来源：http://dih.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fdg.yj20258.top

Ruby: class Admin < User; end
来源：http://egx.cashguo.top

C#:   class Admin : User {}
来源：http://rum.shangyingyoupin.top

[G06] 重写方法
来源：http://rjd.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://fny.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jlr.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://srn.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://oef.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://wys.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wql.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://ree.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://kkp.gotoacloud.top

[G07] 调用父类方法
来源：http://moj.316326.xyz

Py:   super().greet()
来源：http://txl.yfazqb.com

PHP:  parent::greet();
来源：http://kzp.yueranfly.top

JS:   super.greet();
来源：http://fee.sufxvd.cn

TS:   super.greet();
来源：http://jgw.jinqigufen.top

Java: super.greet();
来源：http://ybn.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mxr.haohaochexian.top

Ruby: super
来源：http://fom.bjfxy.top

C#:   base.Greet();
来源：http://qke.jiagoushi.top

[G08] 静态方法与属性
来源：http://rwb.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sgt.aizwys.cn

PHP:  public static function f() {}
来源：http://wxt.hammf.cn

JS:   static f() {}
来源：http://rcx.vehdjk.com

TS:   static f(): void {}
来源：http://hki.yj20258888.top

Java: static void f() {}
来源：http://vyo.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://zwv.ehwqpu.com

Ruby: def self.f; end
来源：http://sks.ydzc1.top

C#:   public static void F() {}
来源：http://mon.yj20258.top

[G09] 接口 / 抽象类
来源：http://vin.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://yvf.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ajg.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xvn.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://lfq.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://prw.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://eob.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ytj.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://hnm.birdmap.top

[G10] 访问控制
来源：http://gxx.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://esv.meibo888.top

PHP:  public / protected / private
来源：http://xtl.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://wux.jinqigufen.top

TS:   public / protected / private
来源：http://lwk.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://rnj.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cnq.mhx1999.top

Ruby: public / protected / private
来源：http://lcf.mhx1999.top

C#:   public / protected / private / internal
来源：http://frs.chenjidiqi.icu

[G11] getter / setter
来源：http://ali.sysykeji.top

Py:   @property 与 @x.setter
来源：http://nel.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://sjk.bbcook.cn

JS:   get name() { return this._name; }
来源：http://lcn.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://kxc.jiagoushi.top

Java: public String getName() { return name; }
来源：http://dmx.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jbu.hywenlv.cn

Ruby: attr_accessor :name
来源：http://vlp.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://svp.hongshengwenyu.top

[G12] 对象转字符串
来源：http://irf.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://koz.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://scu.ivvv.top

JS:   toString() { return this.name; }
来源：http://wdq.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://dpd.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://ren.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fzk.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://vva.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://zua.shzxlz.cn

[G13] 判断对象类型
来源：http://lvh.hcnkem.com

Py:   isinstance(u, User)
来源：http://wro.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://gto.ydzc1.top

JS:   u instanceof User
来源：http://dhd.xuetiantiany.cn

TS:   u instanceof User
来源：http://vbm.aizwys.cn

Java: u instanceof User
来源：http://ygg.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://geh.daria6918.cn

Ruby: u.is_a?(User)
来源：http://puu.yfazqb.com

C#:   u is User
来源：http://njq.shuidangran.top

[G14] 数据类 / record
来源：http://ehe.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mqj.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://pof.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://twn.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://lpk.yuxming.cn

Java: record User(String name, int age) {}
来源：http://kxe.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://ink.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://haf.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://kjr.zhoulong.xyz

[G15] 枚举
来源：http://cmm.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zut.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://szo.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wzo.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xxw.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://azk.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xmc.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://end.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nxk.zhijiandao.cn

[G16] 对象转数组 / 字典
来源：http://knz.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://soh.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://cwl.fehbvm.com

JS:   Object.entries(obj)
来源：http://cfu.snrcjt.cn

TS:   Object.entries(obj)
来源：http://amd.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gqz.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qcc.zycfv.cn

Ruby: obj.instance_variables
来源：http://prs.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://pvd.zhijiandao.cn

================================================================================
来源：http://qde.hesvh.cn

H. 异常与错误处理
来源：http://hmg.haohaochexian.top

================================================================================
来源：http://ktz.zhixingplan.top

[H01] try / catch 基础
来源：http://mwr.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kfj.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rcv.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ubb.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kgz.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://quj.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uuw.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dmi.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gpf.xylfe.cn

[H02] finally / ensure 收尾
来源：http://cqo.fanxiaobao.xyz


<!-- 参考信息 -->