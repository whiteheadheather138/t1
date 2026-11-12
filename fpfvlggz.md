代发 wailian999

Ruby: s.lines
来源：http://fgq.tarul.cn

C#:   s.Split('\n')
来源：http://uut.havefunace.top

[E20] 判断字符串是否为空
来源：http://vhu.feifeiyinyue.top

Py:   if not s:
来源：http://bot.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sly.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jbb.cqqwz.cn

TS:   if (s === "") {}
来源：http://pbr.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://ttl.iojbl.cn

Go:   if s == "" {}
来源：http://kfu.hongshengwenyu.top

Ruby: if s.empty?
来源：http://tjd.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zkh.zycfv.cn

[E21] 超长截断加省略号
来源：http://hgq.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ina.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kds.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nhd.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkh.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://irz.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://pag.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jsw.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mlc.hesvh.cn

[E22] 字节长度与字符长度
来源：http://tbm.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lzn.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bng.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hih.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jud.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gdw.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fiz.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://xng.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dcx.zhiwuduotai.top

================================================================================
来源：http://lzb.bjfxy.top

F. 文件与目录
来源：http://jhb.sxryk.cn

================================================================================
来源：http://obz.chenjidiqi.icu

[F01] 读取整个文件
来源：http://qnn.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pyn.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://lre.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://elg.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lbd.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uqe.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sku.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://bpu.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://phk.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://ojm.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fho.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://idg.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixy.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gtt.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mkn.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cpj.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nnw.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qpl.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://ikf.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gws.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://arw.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jyg.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://otz.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jzt.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vrq.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://wza.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://boz.sjlbkw.cn

[F04] 追加写入文件
来源：http://jlx.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fwi.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gtl.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ixc.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fkn.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aln.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://suk.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dar.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mrz.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://pvf.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zvo.yongpay.top

PHP:  file_exists("a.txt");
来源：http://hap.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://szk.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://vfy.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vfs.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ets.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://vuc.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://xun.uphjek.com

[F06] 删除文件
来源：http://lix.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://qsz.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://shg.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://xsn.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://lze.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://clg.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://dcd.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://ojt.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://rhi.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://gcb.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://drv.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lip.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtv.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aao.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://epg.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bqr.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vki.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iiz.gaohongyu789.top

[F08] 遍历目录
来源：http://tgt.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gqt.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://igk.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://ihg.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://ogu.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gpn.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bfq.sweek.top

Ruby: Dir.children("dir")
来源：http://rrq.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://rgg.zdqjudy.top

[F09] 获取文件大小
来源：http://vco.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://uto.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://hap.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://orq.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://klk.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://yze.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hxu.316326.xyz

Ruby: File.size("a.txt")
来源：http://bur.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://sbm.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://lzy.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hya.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tpj.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://myp.fehbvm.com

TS:   path.extname("a.txt")
来源：http://tte.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ngy.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hfq.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zag.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jia.yvedp.cn

[F11] 复制与移动文件
来源：http://xii.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cfu.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://udx.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kte.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bkw.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ihs.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bbx.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vyu.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bbv.feifeiyinyue.top

[F12] CSV 读写
来源：http://bsm.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vma.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wad.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hyx.yuxming.cn

TS:   // 同上
来源：http://jik.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ypz.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fro.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kzr.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://slt.sweek.top

================================================================================
来源：http://cws.tanke756.top

G. 面向对象
来源：http://ysd.zhiwuduotai.top

================================================================================
来源：http://dxd.zdbjq.cn

[G01] 定义类
来源：http://szo.nanxinkj.top

Py:   class User: pass
来源：http://dmb.sysykeji.top

PHP:  class User {}
来源：http://nev.andypj.xyz

JS:   class User {}
来源：http://jue.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://dij.ywan-chungtsiang.top

Java: class User {}
来源：http://udc.sufxvd.cn

Go:   type User struct { Name string }
来源：http://gxt.birdmap.top

Ruby: class User; end
来源：http://khh.aizwys.cn

C#:   class User {}
来源：http://jlu.gzhubu.top

[G02] 构造函数
来源：http://jqd.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://xcb.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://fnv.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://nzl.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://bfc.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://utg.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zor.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://aru.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://dbf.smart0.xyz

[G03] 实例属性
来源：http://bcs.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://zrz.redwolf501.top

PHP:  public string $name = "x";
来源：http://uha.snrcjt.cn

JS:   this.name = "x";
来源：http://zkv.wangshuangyany.cn

TS:   name: string = "x";
来源：http://tln.xinyue.icu

Java: private String name;
来源：http://pgf.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nox.ppjwa.cn

Ruby: @name = "x"
来源：http://erf.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://sda.hywenlv.cn

[G04] 定义方法
来源：http://qwz.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://ihr.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://svw.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://fzg.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://ofy.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://xps.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ekl.tian-w.cn

Ruby: def greet; @name; end
来源：http://zjw.andypj.xyz

C#:   public string Greet() => Name;
来源：http://fqv.zdqjudy.top

[G05] 继承
来源：http://ujj.sysykeji.top

Py:   class Admin(User): pass
来源：http://mfg.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://luu.chenlongwang.top

JS:   class Admin extends User {}
来源：http://ogp.haohaochexian.top

TS:   class Admin extends User {}
来源：http://mox.iojbl.cn

Java: class Admin extends User {}
来源：http://zpl.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hfy.haohaochexian.top

Ruby: class Admin < User; end
来源：http://oyn.cucudq.cn

C#:   class Admin : User {}
来源：http://whs.fehbvm.com

[G06] 重写方法
来源：http://bmf.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://qsw.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cdd.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://egp.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://sxy.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://kie.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xqr.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://zer.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://uhw.hnxiangtu.top

[G07] 调用父类方法
来源：http://eqd.zhijiandao.cn

Py:   super().greet()
来源：http://tjl.fktsv.cn

PHP:  parent::greet();
来源：http://lxm.nwbrower.top

JS:   super.greet();
来源：http://ifg.nwbrower.top

TS:   super.greet();
来源：http://cmy.chenlongwang.top

Java: super.greet();
来源：http://vsn.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gyb.feifeiyinyue.top

Ruby: super
来源：http://khb.daxiang520.top

C#:   base.Greet();
来源：http://jjx.meibo888.top

[G08] 静态方法与属性
来源：http://ett.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fmi.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://sfz.jinqigufen.top

JS:   static f() {}
来源：http://zip.smart0.xyz

TS:   static f(): void {}
来源：http://dld.hysaishi.cn

Java: static void f() {}
来源：http://fif.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tdo.epnwcf.com

Ruby: def self.f; end
来源：http://bqj.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://nbi.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://jfm.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://mwh.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://enk.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ntl.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://avr.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://dab.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://fmh.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fcp.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://ahq.ppjwa.cn

[G10] 访问控制
来源：http://pwo.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://kej.aizwys.cn

PHP:  public / protected / private
来源：http://olr.kuanghao11.cn

JS:   #private 字段；其余公开
来源：http://rfg.chenlongwang.top

TS:   public / protected / private
来源：http://luq.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://kif.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qky.0kj1m.cn

Ruby: public / protected / private
来源：http://tan.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://rea.yuxming.cn

[G11] getter / setter
来源：http://bws.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://ndh.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fcy.nwbrower.top

JS:   get name() { return this._name; }
来源：http://axq.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://dhh.zhengqikj.top

Java: public String getName() { return name; }
来源：http://apf.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xox.daxiang520.top

Ruby: attr_accessor :name
来源：http://nst.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://pkl.sufxvd.cn

[G12] 对象转字符串
来源：http://zle.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://zii.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cma.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://ror.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://grh.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://shb.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fyu.zycfv.cn

Ruby: def to_s; @name; end
来源：http://cji.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://xlj.nanxinkj.top

[G13] 判断对象类型
来源：http://rcb.andypj.xyz

Py:   isinstance(u, User)
来源：http://ydn.redwolf501.top

PHP:  $u instanceof User
来源：http://zht.sxryk.cn

JS:   u instanceof User
来源：http://dgi.tarul.cn

TS:   u instanceof User
来源：http://plh.xuetiantiany.cn

Java: u instanceof User
来源：http://xxd.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hcr.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://crc.feifeiyinyue.top

C#:   u is User
来源：http://jll.pycfn.com

[G14] 数据类 / record
来源：http://ktc.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ten.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://wnq.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://gzh.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://gwr.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://wxv.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://dcl.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wtm.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://iek.fktsv.cn

[G15] 枚举
来源：http://ums.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bmm.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zee.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uws.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wze.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://zgt.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://szy.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://kfa.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kgj.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://kjh.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://axe.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://sxr.shzxlz.cn

JS:   Object.entries(obj)
来源：http://rql.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://myd.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kpm.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jxc.svipenyu.cn

Ruby: obj.instance_variables
来源：http://rcv.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://bgd.iojbl.cn

================================================================================
来源：http://cai.nanxuanxn.top

H. 异常与错误处理
来源：http://fva.hnxiangtu.top

================================================================================
来源：http://qio.yj202588.top

[H01] try / catch 基础
来源：http://gvn.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tja.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efs.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lgz.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ick.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wis.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dic.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xnx.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wan.hammf.cn

[H02] finally / ensure 收尾
来源：http://sni.fktsv.cn


<!-- 参考信息 -->