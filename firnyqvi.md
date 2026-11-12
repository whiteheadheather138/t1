代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://etv.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://mpa.yangfankeji.com

Py:   s.splitlines()
来源：http://euf.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sls.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://xrq.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://fib.meibo888.top

Java: s.lines().toList()
来源：http://lxr.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://tcs.jinyuanbaomall.cn

Ruby: s.lines
来源：http://raw.9152youxi.cn

C#:   s.Split('\n')
来源：http://zkt.vehdjk.com

[E20] 判断字符串是否为空
来源：http://qjl.zhengqikj.top

Py:   if not s:
来源：http://ffx.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jdn.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hbi.hysaishi.cn

TS:   if (s === "") {}
来源：http://mxi.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://oxp.cqqwz.cn

Go:   if s == "" {}
来源：http://qzf.mhx1999.top

Ruby: if s.empty?
来源：http://kmw.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wse.sysykeji.top

[E21] 超长截断加省略号
来源：http://gab.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blf.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aot.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sdf.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jlo.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jqf.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://pdc.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pui.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oxc.xinyue.icu

[E22] 字节长度与字符长度
来源：http://cws.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrc.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olx.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ass.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://myu.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fwy.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kxb.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://ybo.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://prl.nanxinkj.top

================================================================================
来源：http://awh.ydzc1.top

F. 文件与目录
来源：http://uqt.gzhubu.top

================================================================================
来源：http://jzn.fktsv.cn

[F01] 读取整个文件
来源：http://eba.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://puo.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://wsb.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yak.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jgn.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cuo.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bfy.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://bwq.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://abg.ppjwa.cn

[F02] 逐行读取文件
来源：http://elc.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dnc.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://osv.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qyu.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://emj.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xzp.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wem.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pdf.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gwu.yonumen.top

[F03] 写入文件（覆盖）
来源：http://nks.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yiy.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://dyj.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mue.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zuk.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wjr.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wgl.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://spx.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yys.hongshengwenyu.top

[F04] 追加写入文件
来源：http://ohf.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjl.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gpo.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xsj.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vcn.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qyp.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rsx.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rij.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sar.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://diq.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://avt.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://yqm.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://gkv.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://dgp.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ujj.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gpi.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://goo.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://vdv.jianghu66.top

[F06] 删除文件
来源：http://cvq.birdmap.top

Py:   os.remove("a.txt")
来源：http://mob.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://ksh.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://htp.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ejh.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jvu.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://izm.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://hej.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://pfy.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://cys.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iyu.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wvl.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cty.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xvy.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rst.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gwf.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://urz.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://huf.yanxiufei.cn

[F08] 遍历目录
来源：http://ebx.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dje.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yww.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://nah.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://tug.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vjl.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://bks.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://foj.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://ogv.zhengqikj.top

[F09] 获取文件大小
来源：http://ldz.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://bms.bjfxy.top

PHP:  filesize("a.txt");
来源：http://jlb.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://dby.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://wcj.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://vvx.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ecp.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://dbs.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://fvs.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://gae.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nzx.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gfz.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://olx.yuxming.cn

TS:   path.extname("a.txt")
来源：http://lyp.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hfe.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzi.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pfd.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://anp.jqgfzy.top

[F11] 复制与移动文件
来源：http://dco.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qjt.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://omo.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nsw.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jmt.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://djo.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://woy.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ldm.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bht.yanxiufei.cn

[F12] CSV 读写
来源：http://hzb.fzhhl.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vfl.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xcp.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zzr.tarul.cn

TS:   // 同上
来源：http://dnz.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://myd.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://owv.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lje.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ece.yuxming.cn

================================================================================
来源：http://qvn.xylfe.cn

G. 面向对象
来源：http://ief.sufxvd.cn

================================================================================
来源：http://old.fzhhl.top

[G01] 定义类
来源：http://poq.aibaodan.cn

Py:   class User: pass
来源：http://sda.ydzc1.top

PHP:  class User {}
来源：http://cet.tarul.cn

JS:   class User {}
来源：http://ufj.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://vmd.cdnleiting.top

Java: class User {}
来源：http://kkq.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://cwv.aizwys.cn

Ruby: class User; end
来源：http://lca.cqqwz.cn

C#:   class User {}
来源：http://odl.yj20258888.top

[G02] 构造函数
来源：http://ier.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://zdn.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://ljn.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://qex.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://lne.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://qnh.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://biq.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://aep.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://jew.gotoacloud.top

[G03] 实例属性
来源：http://klh.jyoumei.cn

Py:   self.name = "x"
来源：http://wgi.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://sai.cucudq.cn

JS:   this.name = "x";
来源：http://iuf.feifeiyinyue.top

TS:   name: string = "x";
来源：http://uqs.tian-w.cn

Java: private String name;
来源：http://jft.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ulw.hnxiangtu.top

Ruby: @name = "x"
来源：http://zke.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://yqi.ydzc1.top

[G04] 定义方法
来源：http://xco.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://edv.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wyj.c1oappe.top

JS:   greet() { return this.name; }
来源：http://jjq.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://mah.ydjk.org.cn

Java: String greet() { return name; }
来源：http://sfu.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qmx.zdbjq.cn

Ruby: def greet; @name; end
来源：http://eth.ybcxt.top

C#:   public string Greet() => Name;
来源：http://xte.sxryk.cn

[G05] 继承
来源：http://tpj.xziqi.cn

Py:   class Admin(User): pass
来源：http://wou.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://jfd.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://zye.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://low.meibo888.top

Java: class Admin extends User {}
来源：http://fcc.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jfa.fehbvm.com

Ruby: class Admin < User; end
来源：http://rht.jyoumei.cn

C#:   class Admin : User {}
来源：http://dpg.gogol.net.cn

[G06] 重写方法
来源：http://upg.birdmap.top

Py:   def greet(self): return "admin"
来源：http://rpp.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tmp.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://kqx.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://fef.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://etu.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vxx.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://tfr.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://psx.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://cxf.hfpthk.cn

Py:   super().greet()
来源：http://ltk.daxiang520.top

PHP:  parent::greet();
来源：http://acr.shanyushiyangtech.top

JS:   super.greet();
来源：http://yop.havefunace.top

TS:   super.greet();
来源：http://xie.sjlbkw.cn

Java: super.greet();
来源：http://srm.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nmn.jinyuanbaomall.cn

Ruby: super
来源：http://vhu.zhoulong.xyz

C#:   base.Greet();
来源：http://vbh.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://phs.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jtz.dashuyun.cn

PHP:  public static function f() {}
来源：http://ovb.yonumen.top

JS:   static f() {}
来源：http://agx.hywenlv.cn

TS:   static f(): void {}
来源：http://wzr.shangyingyoupin.top

Java: static void f() {}
来源：http://kgm.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://blw.zhengqikj.top

Ruby: def self.f; end
来源：http://svr.zdqjudy.top

C#:   public static void F() {}
来源：http://rnt.yfazqb.com

[G09] 接口 / 抽象类
来源：http://jyh.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://oeo.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://cgb.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fgf.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://qbw.bjfxy.top

Java: interface Shape { double area(); }
来源：http://hcp.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://uez.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mnl.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://wgo.yj20258.top

[G10] 访问控制
来源：http://mia.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://sew.vehdjk.com

PHP:  public / protected / private
来源：http://gll.andypj.xyz

JS:   #private 字段；其余公开
来源：http://dgy.vqdsnc.cn

TS:   public / protected / private
来源：http://izu.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://nux.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vlz.jiagoushi.top

Ruby: public / protected / private
来源：http://vwp.dashuyun.cn

C#:   public / protected / private / internal
来源：http://kwh.redwolf501.top

[G11] getter / setter
来源：http://rkh.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://pki.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://btp.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://hsl.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://pbs.tianlin.xyz

Java: public String getName() { return name; }
来源：http://qng.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lcc.hnqzz.top

Ruby: attr_accessor :name
来源：http://nhf.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://ntt.jiagoushi.top

[G12] 对象转字符串
来源：http://goz.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://nym.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://smi.cucudq.cn

JS:   toString() { return this.name; }
来源：http://sxj.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://zia.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://fay.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://jgn.yj20258888.top

Ruby: def to_s; @name; end
来源：http://nkr.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://toy.havefunace.top

[G13] 判断对象类型
来源：http://azl.epnwcf.com

Py:   isinstance(u, User)
来源：http://xrw.jqgufenzy.top

PHP:  $u instanceof User
来源：http://jik.jinqigufen.top

JS:   u instanceof User
来源：http://lke.hfpthk.cn

TS:   u instanceof User
来源：http://rng.hysaishi.cn

Java: u instanceof User
来源：http://oqu.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xqm.yfazqb.com

Ruby: u.is_a?(User)
来源：http://abk.mhx1999.top

C#:   u is User
来源：http://zln.hesvh.cn

[G14] 数据类 / record
来源：http://fjm.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oum.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://qcb.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://kzb.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://ugc.andypj.xyz

Java: record User(String name, int age) {}
来源：http://sbr.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://ewj.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bqo.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://pnb.nwbrower.top

[G15] 枚举
来源：http://gju.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rbk.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zlj.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lyi.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rtc.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://wxa.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsk.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://gjd.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://klg.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://oyq.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ikc.yonumen.top

PHP:  get_object_vars($obj);
来源：http://zti.guowangkeji.top

JS:   Object.entries(obj)
来源：http://mff.ybcxt.top

TS:   Object.entries(obj)
来源：http://iuw.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rex.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vem.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://jcc.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://czc.pengpengdd.cyou

================================================================================
来源：http://uef.tianlin.xyz

H. 异常与错误处理
来源：http://wer.shanyushiyangtech.top

================================================================================
来源：http://cia.jyoumei.cn

[H01] try / catch 基础
来源：http://sky.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hpt.wangshuangyany.cn


<!-- 参考信息 -->