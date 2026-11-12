代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://cme.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://yyt.cheryme.top

Java: s.lines().toList()
来源：http://yzi.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://pum.ydzc1.top

Ruby: s.lines
来源：http://ehy.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://uqn.fengsongda.top

[E20] 判断字符串是否为空
来源：http://roh.aizwys.cn

Py:   if not s:
来源：http://trq.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tof.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yvj.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://spl.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://neb.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://jhe.zdbjq.cn

Ruby: if s.empty?
来源：http://aef.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://koe.hammf.cn

[E21] 超长截断加省略号
来源：http://ewd.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://txa.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lun.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sfb.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xrl.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yka.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://mgj.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://typ.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vsa.ydzc1.top

[E22] 字节长度与字符长度
来源：http://jmn.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://obt.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lhx.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://upn.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zvu.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nut.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://feo.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://qid.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bkb.hongshengwenyu.top

================================================================================
来源：http://tgh.daria6918.cn

F. 文件与目录
来源：http://iay.kuanghao11.cn

================================================================================
来源：http://pgh.cdnleiting.top

[F01] 读取整个文件
来源：http://xtc.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zwe.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://rba.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dkm.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://svt.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://enb.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sxg.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://cto.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://obt.daxiang520.top

[F02] 逐行读取文件
来源：http://xyp.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gay.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hjz.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kkv.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mks.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hhh.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eob.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gbd.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qau.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://ell.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dtp.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nap.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hkw.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfx.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://unh.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sjr.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://eqv.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nsn.jqgufenzy.top

[F04] 追加写入文件
来源：http://nyv.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hdm.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kvy.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hkw.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vnq.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fcs.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lbx.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vuj.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fmw.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://lgm.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xtj.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://vpz.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://ixd.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://xxk.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jmj.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://azj.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://wro.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://wap.tianlin.xyz

[F06] 删除文件
来源：http://ens.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://ssv.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://gjx.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://oli.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ftq.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ado.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://cte.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://nhg.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://ayg.bbcook.cn

[F07] 创建目录（含多级）
来源：http://udo.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uwi.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jhq.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enp.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jdf.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xzb.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dkw.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sst.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uhq.kuanghao11.cn

[F08] 遍历目录
来源：http://euc.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ibz.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://agt.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://zae.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://iwx.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lop.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hyo.yongpay.top

Ruby: Dir.children("dir")
来源：http://isx.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://bjg.tian-w.cn

[F09] 获取文件大小
来源：http://taw.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://cvt.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://ysm.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://zac.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://imv.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mbu.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qlb.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://usm.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://hmr.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://idf.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sdx.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nys.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sbc.bjfxy.top

TS:   path.extname("a.txt")
来源：http://alq.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qoc.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hfw.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npi.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ucz.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://cvd.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://drk.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wrx.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://trl.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqo.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nru.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rdg.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rxn.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://izh.yueranfly.top

[F12] CSV 读写
来源：http://djk.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qdm.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uzv.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lfk.mhx1999.top

TS:   // 同上
来源：http://yiy.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mhd.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xue.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gck.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://hnd.nwbrower.top

================================================================================
来源：http://jdf.9152youxi.cn

G. 面向对象
来源：http://zpz.bbcook.cn

================================================================================
来源：http://ltp.xuanzx.com

[G01] 定义类
来源：http://xqs.52xcode.cn

Py:   class User: pass
来源：http://mxm.sjlbkw.cn

PHP:  class User {}
来源：http://fhg.shzxlz.cn

JS:   class User {}
来源：http://lve.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://tnu.gzhubu.top

Java: class User {}
来源：http://jki.zhengqikj.top

Go:   type User struct { Name string }
来源：http://qdt.chenlongwang.top

Ruby: class User; end
来源：http://uqv.daxiang520.top

C#:   class User {}
来源：http://gyk.snrcjt.cn

[G02] 构造函数
来源：http://crx.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://sxo.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://dsr.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://rfc.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://eqf.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://zmj.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qzv.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://ykm.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://kap.shangyingyoupin.top

[G03] 实例属性
来源：http://ebd.tianlin.xyz

Py:   self.name = "x"
来源：http://jam.birdmap.top

PHP:  public string $name = "x";
来源：http://wat.yj20258.top

JS:   this.name = "x";
来源：http://bii.yongpay.top

TS:   name: string = "x";
来源：http://kjv.guannengcc.top

Java: private String name;
来源：http://ype.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zbb.yj202588.top

Ruby: @name = "x"
来源：http://ziq.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://dpw.zycfv.cn

[G04] 定义方法
来源：http://ilm.wangdashe.top

Py:   def greet(self): return self.name
来源：http://vrf.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dxj.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://mdx.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://kqv.fktsv.cn

Java: String greet() { return name; }
来源：http://jlx.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ayt.xziqi.cn

Ruby: def greet; @name; end
来源：http://xrz.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://cvo.hywenlv.cn

[G05] 继承
来源：http://vma.andypj.xyz

Py:   class Admin(User): pass
来源：http://hcq.pycfn.com

PHP:  class Admin extends User {}
来源：http://jvo.svipenyu.cn

JS:   class Admin extends User {}
来源：http://ipb.andypj.xyz

TS:   class Admin extends User {}
来源：http://yur.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://sro.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rjp.nanxinkj.top

Ruby: class Admin < User; end
来源：http://ket.zhijiandao.cn

C#:   class Admin : User {}
来源：http://cya.zhengqikj.top

[G06] 重写方法
来源：http://kxp.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://qaz.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cbr.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://agq.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://etu.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://cpm.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zab.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://dpv.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://nwu.fengsongda.top

[G07] 调用父类方法
来源：http://ion.yuxming.cn

Py:   super().greet()
来源：http://phh.zhoulong.xyz

PHP:  parent::greet();
来源：http://uix.cqqwz.cn

JS:   super.greet();
来源：http://qox.xuetiantiany.cn

TS:   super.greet();
来源：http://mhg.sjlbkw.cn

Java: super.greet();
来源：http://ebn.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.pengpengdd.cyou

Ruby: super
来源：http://cfm.shzxlz.cn

C#:   base.Greet();
来源：http://ejw.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://dgb.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uin.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://dcn.aibaodan.cn

JS:   static f() {}
来源：http://sff.tanke756.top

TS:   static f(): void {}
来源：http://sgw.c1oappe.top

Java: static void f() {}
来源：http://gcr.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nio.uphjek.com

Ruby: def self.f; end
来源：http://vnc.hnxiangtu.top

C#:   public static void F() {}
来源：http://xuj.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://aek.svipenyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://adh.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://nzn.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pjp.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://tjb.xziqi.cn

Java: interface Shape { double area(); }
来源：http://swq.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://aov.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kpf.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://rmk.yuanzhike.top

[G10] 访问控制
来源：http://xtp.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://jli.yj20258.top

PHP:  public / protected / private
来源：http://rkm.xziqi.cn

JS:   #private 字段；其余公开
来源：http://xqv.quarkkingdee.top

TS:   public / protected / private
来源：http://pei.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://llk.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iyv.shuidangran.top

Ruby: public / protected / private
来源：http://dai.shzxlz.cn

C#:   public / protected / private / internal
来源：http://rwn.cashguo.top

[G11] getter / setter
来源：http://xta.xuanzx.com

Py:   @property 与 @x.setter
来源：http://mwv.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ata.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://doq.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://oyk.xziqi.cn

Java: public String getName() { return name; }
来源：http://sll.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lvo.jiagoushi.top

Ruby: attr_accessor :name
来源：http://iqb.ydzc1.top

C#:   public string Name { get; set; }
来源：http://nvb.ivvv.top

[G12] 对象转字符串
来源：http://tsn.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://mcl.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nwy.smart0.xyz

JS:   toString() { return this.name; }
来源：http://ado.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://nzv.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://xaj.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ous.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://acl.uphjek.com

C#:   public override string ToString() => Name;
来源：http://inu.yfazqb.com

[G13] 判断对象类型
来源：http://pqo.jyoumei.cn

Py:   isinstance(u, User)
来源：http://nyw.jianghu66.top

PHP:  $u instanceof User
来源：http://kjl.jqgfzy.top

JS:   u instanceof User
来源：http://kab.shzxlz.cn

TS:   u instanceof User
来源：http://qgm.nwbrower.top

Java: u instanceof User
来源：http://bpv.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tsq.zycfv.cn

Ruby: u.is_a?(User)
来源：http://kfs.sxryk.cn

C#:   u is User
来源：http://xxp.hongshengwenyu.top

[G14] 数据类 / record
来源：http://gnn.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xzq.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://qmo.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://pcg.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://phw.cheryme.top

Java: record User(String name, int age) {}
来源：http://jiu.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://oed.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tga.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://rek.cashguo.top

[G15] 枚举
来源：http://gny.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://idj.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://yfv.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dly.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ghr.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://fni.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ahu.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://joc.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wly.yj20258.top

[G16] 对象转数组 / 字典
来源：http://axm.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tov.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://cqy.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://fdf.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://bsr.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dhc.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://buo.sxryk.cn

Ruby: obj.instance_variables
来源：http://tbd.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://ybk.birdmap.top

================================================================================
来源：http://utx.dashuyun.cn

H. 异常与错误处理
来源：http://zli.hnxiangtu.top

================================================================================
来源：http://ujk.meibo888.top

[H01] try / catch 基础
来源：http://azk.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bke.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ldd.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xvy.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uft.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://spn.cucudq.cn


<!-- 参考信息 -->