代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://pcf.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xwr.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ipx.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tbu.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vmw.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://irt.yongpay.top

Py:   s.splitlines()
来源：http://dmr.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wqd.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://bus.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://jdl.yj20258.top

Java: s.lines().toList()
来源：http://xuj.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://jrh.jinqigufen.top

Ruby: s.lines
来源：http://pug.zhoulong.xyz

C#:   s.Split('\n')
来源：http://yon.yvedp.cn

[E20] 判断字符串是否为空
来源：http://rak.zdqjudy.top

Py:   if not s:
来源：http://zdw.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ftk.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gvy.shuidangran.top

TS:   if (s === "") {}
来源：http://zbl.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://gwq.xinyue.icu

Go:   if s == "" {}
来源：http://cjs.bjfxy.top

Ruby: if s.empty?
来源：http://aeb.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zoz.pycfn.com

[E21] 超长截断加省略号
来源：http://tyl.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bjp.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yqk.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://twj.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://old.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahu.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://scq.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cow.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cxv.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://eeo.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eyo.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zhl.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://grt.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mkd.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bps.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fgd.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://ytq.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lqp.shanyushiyangkeji.top

================================================================================
来源：http://lzl.redwolf501.top

F. 文件与目录
来源：http://yht.pengpengdd.cyou

================================================================================
来源：http://cbh.aizwys.cn

[F01] 读取整个文件
来源：http://anl.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hze.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://hab.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ncw.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vwz.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://fps.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://koy.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://mss.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://rvg.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://uzo.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gty.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ktq.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qak.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fim.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zgd.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uvl.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ckm.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uka.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://ydu.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iyk.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ixs.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nfa.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxc.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mph.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ggj.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://sdg.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://avb.jyoumei.cn

[F04] 追加写入文件
来源：http://pjj.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://muy.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oqn.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewk.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://awm.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ooy.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://frj.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mzs.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uva.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://ezb.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://syz.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://pyp.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://vzl.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://qrg.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nje.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sxp.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://cth.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://bqe.sxryk.cn

[F06] 删除文件
来源：http://kor.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://mxv.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://cjd.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yge.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://zhr.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ofk.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://dxw.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://akr.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://uqg.jianghu66.top

[F07] 创建目录（含多级）
来源：http://auh.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qru.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jvi.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vlk.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nnz.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kuj.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tij.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nwl.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qoa.aibaodan.cn

[F08] 遍历目录
来源：http://tnb.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mmb.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kxr.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://scn.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://bly.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dlz.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hip.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://cga.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://thv.nwbrower.top

[F09] 获取文件大小
来源：http://hlm.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://osj.zycfv.cn

PHP:  filesize("a.txt");
来源：http://qra.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://sek.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://tpc.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://iob.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lad.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://hxh.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://rge.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://dzj.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://knx.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tsi.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://owj.aizwys.cn

TS:   path.extname("a.txt")
来源：http://iks.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pls.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zsb.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xqw.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qff.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://onz.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kfm.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpt.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hir.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jce.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obc.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sbm.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qdw.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wrr.vqdsnc.cn

[F12] CSV 读写
来源：http://boc.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://afn.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rvi.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zil.yongpay.top

TS:   // 同上
来源：http://mao.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bkw.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iao.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://unm.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kpr.sweek.top

================================================================================
来源：http://orq.jyoumei.cn

G. 面向对象
来源：http://qzn.xziqi.cn

================================================================================
来源：http://gzf.tanke756.top

[G01] 定义类
来源：http://gkw.jiagoushi.top

Py:   class User: pass
来源：http://bkz.yj20258.top

PHP:  class User {}
来源：http://sei.chenlongwang.top

JS:   class User {}
来源：http://tzi.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://ans.uphjek.com

Java: class User {}
来源：http://svb.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://wgt.bbcook.cn

Ruby: class User; end
来源：http://rae.jiagoushi.top

C#:   class User {}
来源：http://ibp.tianlin.xyz

[G02] 构造函数
来源：http://tuk.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://qfa.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://nkj.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://xox.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://yev.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://bsd.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rzx.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://tsf.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://rab.iojbl.cn

[G03] 实例属性
来源：http://dwy.zhijiandao.cn

Py:   self.name = "x"
来源：http://iuk.fktsv.cn

PHP:  public string $name = "x";
来源：http://hsf.vehdjk.com

JS:   this.name = "x";
来源：http://dpg.yuanzhike.top

TS:   name: string = "x";
来源：http://rut.svipenyu.cn

Java: private String name;
来源：http://vrt.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://izq.feifeiyinyue.top

Ruby: @name = "x"
来源：http://uay.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://ayh.nanxinkj.top

[G04] 定义方法
来源：http://gxq.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://xrz.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tbw.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://jlx.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://wab.dianchejie.cn

Java: String greet() { return name; }
来源：http://ffd.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://udm.nwbrower.top

Ruby: def greet; @name; end
来源：http://ozb.birdmap.top

C#:   public string Greet() => Name;
来源：http://jhi.xziqi.cn

[G05] 继承
来源：http://awl.wangdashe.top

Py:   class Admin(User): pass
来源：http://zai.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://osw.sweek.top

JS:   class Admin extends User {}
来源：http://xpb.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://mmk.uphjek.com

Java: class Admin extends User {}
来源：http://vki.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gyi.ivvv.top

Ruby: class Admin < User; end
来源：http://odi.sxryk.cn

C#:   class Admin : User {}
来源：http://rva.cashguo.top

[G06] 重写方法
来源：http://qsa.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://mpm.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://slk.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://fjp.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://khg.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://fbc.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xqv.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://now.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://taj.guannengcc.top

[G07] 调用父类方法
来源：http://qgi.xuetiantiany.cn

Py:   super().greet()
来源：http://bpg.zhiwuduotai.top

PHP:  parent::greet();
来源：http://you.hnqzz.top

JS:   super.greet();
来源：http://gvl.jqgufenzy.top

TS:   super.greet();
来源：http://dlw.vqdsnc.cn

Java: super.greet();
来源：http://avm.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mpi.yvedp.cn

Ruby: super
来源：http://fep.chenjidiqi.icu

C#:   base.Greet();
来源：http://wiz.0kj1m.cn

[G08] 静态方法与属性
来源：http://mbi.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pvk.chenlongwang.top

PHP:  public static function f() {}
来源：http://dzz.tarul.cn

JS:   static f() {}
来源：http://qae.cdnleiting.top

TS:   static f(): void {}
来源：http://wyw.smart0.xyz

Java: static void f() {}
来源：http://sqt.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zyk.ctjpmb.com

Ruby: def self.f; end
来源：http://dyu.sweek.top

C#:   public static void F() {}
来源：http://qqc.52xcode.cn

[G09] 接口 / 抽象类
来源：http://giz.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://tab.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://aoe.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fpd.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://mts.cheryme.top

Java: interface Shape { double area(); }
来源：http://dcp.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://ect.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xnw.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://cln.hfpthk.cn

[G10] 访问控制
来源：http://tic.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://zlj.snrcjt.cn

PHP:  public / protected / private
来源：http://qub.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://pyn.sxryk.cn

TS:   public / protected / private
来源：http://phg.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://hbu.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ofu.fengsongda.top

Ruby: public / protected / private
来源：http://wmm.316326.xyz

C#:   public / protected / private / internal
来源：http://drl.fanxiaobao.xyz

[G11] getter / setter
来源：http://ibb.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://nrr.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pwf.hnqzz.top

JS:   get name() { return this._name; }
来源：http://ljz.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://deg.tarul.cn

Java: public String getName() { return name; }
来源：http://ldl.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gsx.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://xkw.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://sya.yvedp.cn

[G12] 对象转字符串
来源：http://wyb.yongpay.top

Py:   def __str__(self): return self.name
来源：http://bfa.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nrw.shuidangran.top

JS:   toString() { return this.name; }
来源：http://dtn.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://uoe.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://ypg.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://pst.gzhubu.top

Ruby: def to_s; @name; end
来源：http://fla.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://hux.yuanzhike.top

[G13] 判断对象类型
来源：http://oxm.zdqjudy.top

Py:   isinstance(u, User)
来源：http://lmy.0kj1m.cn

PHP:  $u instanceof User
来源：http://rpl.cqqwz.cn

JS:   u instanceof User
来源：http://cxs.c1oappe.top

TS:   u instanceof User
来源：http://dxs.feifeiyinyue.top

Java: u instanceof User
来源：http://kwy.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ons.yongpay.top

Ruby: u.is_a?(User)
来源：http://cto.xziqi.cn

C#:   u is User
来源：http://dxk.epnwcf.com

[G14] 数据类 / record
来源：http://zlm.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vzy.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://vbd.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lpv.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://qrp.tanke756.top

Java: record User(String name, int age) {}
来源：http://uls.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://kvy.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ejn.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://ifo.feifeiyinyue.top

[G15] 枚举
来源：http://yrs.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://amb.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sqc.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://smt.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ytv.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://dyd.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqi.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://pgz.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wbe.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://ybl.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wur.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://tia.xuanzx.com

JS:   Object.entries(obj)
来源：http://vyv.vehdjk.com

TS:   Object.entries(obj)
来源：http://umh.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qsp.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nyy.ybcxt.top

Ruby: obj.instance_variables
来源：http://oka.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://lqb.shanyushiyangtech.top

================================================================================
来源：http://olp.ehwqpu.com


<!-- 参考信息 -->