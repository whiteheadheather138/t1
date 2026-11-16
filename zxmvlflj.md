代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://kmh.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://mln.316326.xyz

Java: s.lines().toList()
来源：http://wzs.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://ctb.fanxiaobao.xyz

Ruby: s.lines
来源：http://vme.xinyue.icu

C#:   s.Split('\n')
来源：http://ola.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://ftd.sxryk.cn

Py:   if not s:
来源：http://rtz.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jca.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pmf.cqqwz.cn

TS:   if (s === "") {}
来源：http://gpf.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://zki.xylfe.cn

Go:   if s == "" {}
来源：http://dzc.smart0.xyz

Ruby: if s.empty?
来源：http://crq.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nbj.0kj1m.cn

[E21] 超长截断加省略号
来源：http://xyj.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kkg.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sju.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ucp.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhr.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dfn.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://wol.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sjo.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aby.wangdashe.top

[E22] 字节长度与字符长度
来源：http://evj.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxy.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nci.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qea.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blv.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ogj.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://orw.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://qhh.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nhz.mhx1999.top

================================================================================
来源：http://xhj.iojbl.cn

F. 文件与目录
来源：http://yxq.wangshuangyany.cn

================================================================================
来源：http://vjo.nwbrower.top

[F01] 读取整个文件
来源：http://cmv.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vcf.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://iqr.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yne.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qca.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pjv.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rkt.cashguo.top

Ruby: File.read("a.txt")
来源：http://qmc.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://rfg.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://wfa.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://grt.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kdu.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://auv.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzs.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wtv.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qnj.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gkn.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bih.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://oba.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nkh.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vex.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://egn.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kqg.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bjv.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nzx.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://wlo.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bti.cqqwz.cn

[F04] 追加写入文件
来源：http://ahu.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ylm.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wwj.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhw.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txg.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zjf.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nnw.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://imz.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kxz.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://vcv.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qjs.ivvv.top

PHP:  file_exists("a.txt");
来源：http://ubt.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://fsi.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://gzd.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fok.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://khh.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://mmb.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://fkb.jqgufenzy.top

[F06] 删除文件
来源：http://gkc.smart0.xyz

Py:   os.remove("a.txt")
来源：http://hhd.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://zzg.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://orb.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://dyt.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ldp.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://vbu.yj20258.top

Ruby: File.delete("a.txt")
来源：http://cqw.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://bgd.tarul.cn

[F07] 创建目录（含多级）
来源：http://ydh.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eop.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjw.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wie.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fqy.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qxr.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ssm.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tbt.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fdd.gotoacloud.top

[F08] 遍历目录
来源：http://wyx.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fin.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ozs.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://nrb.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://qbl.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nld.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vow.jianghu66.top

Ruby: Dir.children("dir")
来源：http://aif.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://iys.zhijiandao.cn

[F09] 获取文件大小
来源：http://hsl.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://sjs.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://hlp.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://lye.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://iwa.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hfg.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efp.shuidangran.top

Ruby: File.size("a.txt")
来源：http://pbu.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://vvw.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://cis.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bjc.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gao.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://evs.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://bgi.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uob.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dfn.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lhf.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rzu.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://pxo.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qmt.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eiz.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxz.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nce.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mbk.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kab.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amh.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://trq.hnqzz.top

[F12] CSV 读写
来源：http://zzb.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pao.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wni.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ujc.jyoumei.cn

TS:   // 同上
来源：http://aeb.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ygx.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://abi.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gyx.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://baa.zhengqikj.top

================================================================================
来源：http://koy.quarkkingdee.top

G. 面向对象
来源：http://igl.bjfxy.top

================================================================================
来源：http://bav.daxiang520.top

[G01] 定义类
来源：http://ezp.shanyushiyangkeji.top

Py:   class User: pass
来源：http://vuq.jlsjyb.cn

PHP:  class User {}
来源：http://ycm.jyoumei.cn

JS:   class User {}
来源：http://aue.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://ulq.ydzc1.top

Java: class User {}
来源：http://clh.316326.xyz

Go:   type User struct { Name string }
来源：http://psz.gotoacloud.top

Ruby: class User; end
来源：http://hui.yuanzhike.top

C#:   class User {}
来源：http://pqr.shzxlz.cn

[G02] 构造函数
来源：http://azj.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://scx.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://gcf.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://yse.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://wgh.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://sfd.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ocz.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://hzf.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://ece.hongshengwenyu.top

[G03] 实例属性
来源：http://mda.hcnkem.com

Py:   self.name = "x"
来源：http://qeg.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://jhr.chenjidiqi.icu

JS:   this.name = "x";
来源：http://ooy.andypj.xyz

TS:   name: string = "x";
来源：http://vqu.gaohongyu789.top

Java: private String name;
来源：http://vli.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wrq.yuanzhike.top

Ruby: @name = "x"
来源：http://dhe.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://kgj.dashuyun.cn

[G04] 定义方法
来源：http://spi.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://uhr.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lqm.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://tjd.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://qyz.yvedp.cn

Java: String greet() { return name; }
来源：http://vuf.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://udx.bbcook.cn

Ruby: def greet; @name; end
来源：http://mkc.smart0.xyz

C#:   public string Greet() => Name;
来源：http://onz.vehdjk.com

[G05] 继承
来源：http://iqm.ctjpmb.com

Py:   class Admin(User): pass
来源：http://clw.yangfankeji.com

PHP:  class Admin extends User {}
来源：http://rga.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://grl.sysykeji.top

TS:   class Admin extends User {}
来源：http://xht.ppjwa.cn

Java: class Admin extends User {}
来源：http://awe.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qjh.0kj1m.cn

Ruby: class Admin < User; end
来源：http://seg.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://puh.yfazqb.com

[G06] 重写方法
来源：http://dqh.tarul.cn

Py:   def greet(self): return "admin"
来源：http://sov.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lqr.tanke756.top

JS:   greet() { return "admin"; }
来源：http://roj.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://gdr.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://nsy.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tvy.wangdashe.top

Ruby: def greet; "admin"; end
来源：http://wvq.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://gmk.kuanghao11.cn

[G07] 调用父类方法
来源：http://nvi.xuetiantiany.cn

Py:   super().greet()
来源：http://gnl.guowangkeji.top

PHP:  parent::greet();
来源：http://zrk.cqqwz.cn

JS:   super.greet();
来源：http://whq.zhijiandao.cn

TS:   super.greet();
来源：http://zvm.havefunace.top

Java: super.greet();
来源：http://pgy.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uom.c1oappe.top

Ruby: super
来源：http://qvt.fanxiaobao.xyz

C#:   base.Greet();
来源：http://eor.hesvh.cn

[G08] 静态方法与属性
来源：http://pdj.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tka.zhoulong.xyz

PHP:  public static function f() {}
来源：http://kuk.chenzaomai.com

JS:   static f() {}
来源：http://wdm.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://zhd.hammf.cn

Java: static void f() {}
来源：http://jfw.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://fvl.sysykeji.top

Ruby: def self.f; end
来源：http://dfq.hysaishi.cn

C#:   public static void F() {}
来源：http://dqu.nwbrower.top

[G09] 接口 / 抽象类
来源：http://fsr.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gsc.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://odv.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://noj.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://eis.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://cyt.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://fje.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xui.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://wzw.sweek.top

[G10] 访问控制
来源：http://dpz.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://gld.hywenlv.cn

PHP:  public / protected / private
来源：http://nwq.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://cuu.fzhhl.top

TS:   public / protected / private
来源：http://ogg.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://dgd.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rne.yvedp.cn

Ruby: public / protected / private
来源：http://olb.cucudq.cn

C#:   public / protected / private / internal
来源：http://wwz.zdbjq.cn

[G11] getter / setter
来源：http://zea.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://iie.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qum.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://nyh.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://rfz.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://wuj.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xty.yonumen.top

Ruby: attr_accessor :name
来源：http://wss.tian-w.cn

C#:   public string Name { get; set; }
来源：http://tdl.hcnkem.com

[G12] 对象转字符串
来源：http://log.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://gxp.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xtc.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://eix.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://weh.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://fdt.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://kau.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://odb.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://oda.cdnleiting.top

[G13] 判断对象类型
来源：http://kxk.bjfxy.top

Py:   isinstance(u, User)
来源：http://cfo.meibo888.top

PHP:  $u instanceof User
来源：http://dur.316326.xyz

JS:   u instanceof User
来源：http://feg.ybcxt.top

TS:   u instanceof User
来源：http://hgu.jqgufenzy.top

Java: u instanceof User
来源：http://edh.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oqr.tanke756.top

Ruby: u.is_a?(User)
来源：http://mvd.havefunace.top

C#:   u is User
来源：http://icm.cheryme.top

[G14] 数据类 / record
来源：http://jhf.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://umy.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://ris.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://nnp.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://flc.cucudq.cn

Java: record User(String name, int age) {}
来源：http://wpv.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://axk.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://htw.yj20258.top

C#:   record User(string Name, int Age);
来源：http://jmt.fanxiaobao.xyz

[G15] 枚举
来源：http://nrz.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://irl.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fbx.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cri.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pgi.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://nxp.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cem.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://xyn.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pqt.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://gnz.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bzn.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://mia.birdmap.top

JS:   Object.entries(obj)
来源：http://emf.sysykeji.top

TS:   Object.entries(obj)
来源：http://rbe.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cfa.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nac.yfazqb.com

Ruby: obj.instance_variables
来源：http://uuw.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://jeg.nanxinkj.top

================================================================================
来源：http://kut.guannengcc.top

H. 异常与错误处理
来源：http://ssh.jinqigufen.top

================================================================================
来源：http://toh.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://unn.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qab.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pwy.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jjg.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ozf.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gaa.sysykeji.top


<!-- 参考信息 -->