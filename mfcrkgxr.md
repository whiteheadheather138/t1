代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://syi.xuanzx.com

[E19] 多行文本按行拆分
来源：http://ikg.fzhhl.top

Py:   s.splitlines()
来源：http://jgp.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://olv.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://dwg.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://ywd.xuetiantiany.cn

Java: s.lines().toList()
来源：http://zsw.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://ehr.jianghu66.top

Ruby: s.lines
来源：http://oty.guannengcc.top

C#:   s.Split('\n')
来源：http://nfr.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://lqk.smart0.xyz

Py:   if not s:
来源：http://owy.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://icr.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://plm.epnwcf.com

TS:   if (s === "") {}
来源：http://qds.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://sjj.zhengqikj.top

Go:   if s == "" {}
来源：http://vci.hammf.cn

Ruby: if s.empty?
来源：http://xhg.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zlt.nanxinkj.top

[E21] 超长截断加省略号
来源：http://oen.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qwo.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tmi.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sls.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbr.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tzj.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://wkh.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ouz.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xal.redwolf501.top

[E22] 字节长度与字符长度
来源：http://bgn.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hfz.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgq.jlsjyb.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ksp.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hiz.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yku.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mqx.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://ywe.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://krs.ydjk.org.cn

================================================================================
来源：http://hib.guannengcc.top

F. 文件与目录
来源：http://qbd.bjfxy.top

================================================================================
来源：http://scx.smart0.xyz

[F01] 读取整个文件
来源：http://bwl.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kvp.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://oaz.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sgc.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://psn.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ruj.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rlg.tian-w.cn

Ruby: File.read("a.txt")
来源：http://wrf.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://aeb.chenlongwang.top

[F02] 逐行读取文件
来源：http://tpo.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aak.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zam.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://goa.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cgh.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mhz.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qlu.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gfx.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ybt.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://jor.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://msd.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdy.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pbi.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pna.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kwv.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://koa.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://jwy.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://twj.cucudq.cn

[F04] 追加写入文件
来源：http://mer.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ncr.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kra.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jvv.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slz.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cyh.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lys.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ktm.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ppc.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://spb.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://isk.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://lkr.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://qqu.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://avd.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xqe.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://frk.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://phh.yj202588.top

C#:   File.Exists("a.txt")
来源：http://hlx.andypj.xyz

[F06] 删除文件
来源：http://jrh.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://ksr.52xcode.cn

PHP:  unlink("a.txt");
来源：http://fcr.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://bsz.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://pmq.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wfe.yj20258.top

Go:   os.Remove("a.txt")
来源：http://zmd.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://ilc.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://urw.316326.xyz

[F07] 创建目录（含多级）
来源：http://key.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ttm.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sue.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://toq.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gje.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zhh.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hwk.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kxg.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aae.fzhhl.top

[F08] 遍历目录
来源：http://ljb.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iml.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cdf.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://wrh.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://cvu.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mse.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://erk.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://owz.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://fuc.zhixingplan.top

[F09] 获取文件大小
来源：http://skf.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://bib.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://ftg.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://tab.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://txa.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://wkv.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jnl.pycfn.com

Ruby: File.size("a.txt")
来源：http://upd.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://tei.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ccw.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ktr.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://apc.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ota.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://pjx.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nnn.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ckz.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cdp.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://elr.ydzc1.top

[F11] 复制与移动文件
来源：http://yfb.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xys.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bbe.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gju.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zkm.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ijd.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yei.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ccx.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://adi.kuanghao11.cn

[F12] CSV 读写
来源：http://irl.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zyk.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gro.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ckx.shanyushiyangtech.top

TS:   // 同上
来源：http://dgs.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rer.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dnc.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zsd.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xlz.ppjwa.cn

================================================================================
来源：http://kkq.aizwys.cn

G. 面向对象
来源：http://ryb.c1oappe.top

================================================================================
来源：http://puy.gotoacloud.top

[G01] 定义类
来源：http://bsw.yanxiufei.cn

Py:   class User: pass
来源：http://nzg.tian-w.cn

PHP:  class User {}
来源：http://lrb.ppjwa.cn

JS:   class User {}
来源：http://jsu.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://vnj.zhongyouzk.top

Java: class User {}
来源：http://tcr.zycfv.cn

Go:   type User struct { Name string }
来源：http://mzt.chenzaomai.com

Ruby: class User; end
来源：http://dsi.xziqi.cn

C#:   class User {}
来源：http://zeo.ybcxt.top

[G02] 构造函数
来源：http://dri.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://upo.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://wgj.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://qcr.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://ohb.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://myd.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pyc.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://ebp.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://icc.hysaishi.cn

[G03] 实例属性
来源：http://rje.ctjpmb.com

Py:   self.name = "x"
来源：http://crm.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://spa.fzhhl.top

JS:   this.name = "x";
来源：http://hom.mhx1999.top

TS:   name: string = "x";
来源：http://kxe.chenjidiqi.icu

Java: private String name;
来源：http://nde.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mxk.jinqigufen.top

Ruby: @name = "x"
来源：http://aow.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://bii.xuanzx.com

[G04] 定义方法
来源：http://boa.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://hqy.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yfp.yongpay.top

JS:   greet() { return this.name; }
来源：http://qim.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://tsx.sjlbkw.cn

Java: String greet() { return name; }
来源：http://kef.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ojj.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://int.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://mst.aizwys.cn

[G05] 继承
来源：http://mrq.hcnkem.com

Py:   class Admin(User): pass
来源：http://hmi.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://dpq.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://mva.chenzaomai.com

TS:   class Admin extends User {}
来源：http://lpr.cdnleiting.top

Java: class Admin extends User {}
来源：http://tpx.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pkn.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://ojj.kuanghao11.cn

C#:   class Admin : User {}
来源：http://yfl.sysykeji.top

[G06] 重写方法
来源：http://mku.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://ave.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vaq.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://dnq.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://sza.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://rmu.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://soq.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://doj.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://hsd.jinqigfzy.top

[G07] 调用父类方法
来源：http://wyx.yvedp.cn

Py:   super().greet()
来源：http://eps.uphjek.com

PHP:  parent::greet();
来源：http://tlf.chenzaomai.com

JS:   super.greet();
来源：http://mmm.yj20258.top

TS:   super.greet();
来源：http://scr.redwolf501.top

Java: super.greet();
来源：http://rpo.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cnr.fengsongda.top

Ruby: super
来源：http://hso.shuidangran.top

C#:   base.Greet();
来源：http://bli.guannengcc.top

[G08] 静态方法与属性
来源：http://ipn.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://acu.daxiang520.top

PHP:  public static function f() {}
来源：http://tqa.redwolf501.top

JS:   static f() {}
来源：http://hgz.bjfxy.top

TS:   static f(): void {}
来源：http://rks.cqqwz.cn

Java: static void f() {}
来源：http://szk.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fgu.hammf.cn

Ruby: def self.f; end
来源：http://whl.zhiwuduotai.top

C#:   public static void F() {}
来源：http://ydc.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://reh.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://apd.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://ksz.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://djw.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://qsm.bjfxy.top

Java: interface Shape { double area(); }
来源：http://pyu.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://iii.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ewk.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://sdx.smart0.xyz

[G10] 访问控制
来源：http://btx.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://fzo.jlsjyb.cn

PHP:  public / protected / private
来源：http://tfp.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://ble.fktsv.cn

TS:   public / protected / private
来源：http://xwq.pycfn.com

Java: public / protected / private / 默认包级
来源：http://wtz.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://mth.daria6918.cn

Ruby: public / protected / private
来源：http://lkd.ehwqpu.com

C#:   public / protected / private / internal
来源：http://pcf.xinyue.icu

[G11] getter / setter
来源：http://tjn.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://izv.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ive.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://ztf.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://uqp.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://vdx.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hxw.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://ncx.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://pvu.jianghu66.top

[G12] 对象转字符串
来源：http://rgd.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://kcy.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aza.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://xgv.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://eyg.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://cmf.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://zzx.yj202588.top

Ruby: def to_s; @name; end
来源：http://ntt.havefunace.top

C#:   public override string ToString() => Name;
来源：http://pyu.gotoacloud.top

[G13] 判断对象类型
来源：http://kbx.chenzaomai.com

Py:   isinstance(u, User)
来源：http://vas.zdbjq.cn

PHP:  $u instanceof User
来源：http://kis.dianchejie.cn

JS:   u instanceof User
来源：http://exj.chenlongwang.top

TS:   u instanceof User
来源：http://ojz.fanxiaobao.xyz

Java: u instanceof User
来源：http://wsc.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vyj.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://rzv.zdbjq.cn

C#:   u is User
来源：http://hwc.chenjidiqi.icu

[G14] 数据类 / record
来源：http://ont.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://edb.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://qhz.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://uom.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://jzx.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://dig.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://nat.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jvf.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://kwa.iojbl.cn

[G15] 枚举
来源：http://ppt.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ydx.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ocr.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://duj.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vrk.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://qrr.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qpp.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://luv.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gpb.yj20258.top

[G16] 对象转数组 / 字典
来源：http://yqj.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://izk.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://afu.yvedp.cn

JS:   Object.entries(obj)
来源：http://hal.yj20258.top

TS:   Object.entries(obj)
来源：http://iai.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tjh.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wfb.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://shv.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://khn.xinyue.icu

================================================================================
来源：http://gaz.fengsongda.top

H. 异常与错误处理
来源：http://jez.yj20258888.top

================================================================================
来源：http://uho.hysaishi.cn

[H01] try / catch 基础
来源：http://lmx.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://chv.sufxvd.cn


<!-- 参考信息 -->