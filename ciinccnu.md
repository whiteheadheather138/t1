代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://toc.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ykb.chenjidiqi.icu

Ruby: s.capitalize
来源：http://lfo.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qws.yvedp.cn

[E18] 模板占位符替换
来源：http://jby.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oto.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ssq.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lup.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jxi.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wns.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sdo.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xvh.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uve.yvedp.cn

[E19] 多行文本按行拆分
来源：http://rmq.haohaochexian.top

Py:   s.splitlines()
来源：http://ycd.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rno.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://rri.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://bac.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://crh.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://nlu.xuetiantiany.cn

Ruby: s.lines
来源：http://dia.gzhubu.top

C#:   s.Split('\n')
来源：http://okg.havefunace.top

[E20] 判断字符串是否为空
来源：http://rrf.aizwys.cn

Py:   if not s:
来源：http://imw.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cux.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bxy.aizwys.cn

TS:   if (s === "") {}
来源：http://iop.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://bmi.0kj1m.cn

Go:   if s == "" {}
来源：http://jsw.xylfe.cn

Ruby: if s.empty?
来源：http://snf.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yyl.ctjpmb.com

[E21] 超长截断加省略号
来源：http://zbq.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yam.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zui.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pqv.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://die.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ocy.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://ebu.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fxd.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://woc.xuanzx.com

[E22] 字节长度与字符长度
来源：http://sck.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ckk.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgl.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ppy.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zhv.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mad.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bsz.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://djj.zhiwuduotai.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bac.zhoulong.xyz

================================================================================
来源：http://nvb.ydzc1.top

F. 文件与目录
来源：http://xtt.wangdashe.top

================================================================================
来源：http://eel.uphjek.com

[F01] 读取整个文件
来源：http://vcp.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xqc.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://nwp.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bxf.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ddz.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fku.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://glp.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://qmf.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://fil.tarul.cn

[F02] 逐行读取文件
来源：http://val.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fir.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wyx.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jbm.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aim.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://agm.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kzr.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bek.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nen.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://ajo.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kmi.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://scf.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fbj.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hos.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xzh.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fsq.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ttk.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://adt.jlsjyb.cn

[F04] 追加写入文件
来源：http://waw.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qdd.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mov.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vgk.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmz.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gcn.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fvx.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jlf.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://snc.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://hds.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pcy.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://sic.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://rer.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://lid.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ahn.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://piz.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://evk.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://ukn.jinghuilouyu.cn

[F06] 删除文件
来源：http://qtz.redwolf501.top

Py:   os.remove("a.txt")
来源：http://yxa.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://txv.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pez.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://mqx.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://opn.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://trh.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://yba.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://yxe.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://ufa.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltm.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://waq.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kjh.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nrc.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wzp.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vhm.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bah.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://umq.jinqigufen.top

[F08] 遍历目录
来源：http://aec.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://drc.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dxp.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://rsm.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://uly.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ndw.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dml.hnqzz.top

Ruby: Dir.children("dir")
来源：http://bqt.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://wzg.chenlongwang.top

[F09] 获取文件大小
来源：http://syo.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://yik.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://uyu.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://xja.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://xij.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://rjg.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://epp.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://pti.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://gpu.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://gij.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qwf.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mgh.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ceh.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://gwf.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hdd.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yvj.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pva.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dsb.cashguo.top

[F11] 复制与移动文件
来源：http://gvk.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ias.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lgm.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vgm.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://umn.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rvt.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cdl.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ciw.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pxn.sysykeji.top

[F12] CSV 读写
来源：http://ezx.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lbj.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://akh.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nif.smart0.xyz

TS:   // 同上
来源：http://cud.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://abk.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dky.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uwl.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xbb.9152youxi.cn

================================================================================
来源：http://gjf.hnxiangtu.top

G. 面向对象
来源：http://uop.xuanzx.com

================================================================================
来源：http://ehd.chenzaomai.com

[G01] 定义类
来源：http://bpc.cashguo.top

Py:   class User: pass
来源：http://mlt.jyoumei.cn

PHP:  class User {}
来源：http://rld.jinghuilouyu.cn

JS:   class User {}
来源：http://qix.ivvv.top

TS:   class User { name: string = ""; }
来源：http://wml.jianghu66.top

Java: class User {}
来源：http://qad.yj20258.top

Go:   type User struct { Name string }
来源：http://tgq.shangyingyoupin.top

Ruby: class User; end
来源：http://cqr.daria6918.cn

C#:   class User {}
来源：http://hob.snrcjt.cn

[G02] 构造函数
来源：http://faj.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://lxf.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://odp.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://psm.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://aab.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://onc.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://skx.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://xdc.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://pds.jinyuanbaomall.cn

[G03] 实例属性
来源：http://wue.daria6918.cn

Py:   self.name = "x"
来源：http://tfj.yj20258888.top

PHP:  public string $name = "x";
来源：http://bwz.pengpengdd.cyou

JS:   this.name = "x";
来源：http://erl.ehwqpu.com

TS:   name: string = "x";
来源：http://yzu.xuetiantiany.cn

Java: private String name;
来源：http://gwn.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hyg.jinqigufen.top

Ruby: @name = "x"
来源：http://dip.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://wgt.hfpthk.cn

[G04] 定义方法
来源：http://wdm.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://dje.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pzs.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://cgu.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://ixp.zhoulong.xyz

Java: String greet() { return name; }
来源：http://icc.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lyo.iojbl.cn

Ruby: def greet; @name; end
来源：http://ohe.vehdjk.com

C#:   public string Greet() => Name;
来源：http://cfr.pengpengdd.cyou

[G05] 继承
来源：http://qss.cucudq.cn

Py:   class Admin(User): pass
来源：http://hsr.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://sxv.ppjwa.cn

JS:   class Admin extends User {}
来源：http://rsl.havefunace.top

TS:   class Admin extends User {}
来源：http://vcf.birdmap.top

Java: class Admin extends User {}
来源：http://ctf.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qml.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://nxu.nanxuanxn.top

C#:   class Admin : User {}
来源：http://glb.kuanghao11.cn

[G06] 重写方法
来源：http://cuw.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://uaz.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zts.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://koy.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://wjz.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://lnf.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqg.birdmap.top

Ruby: def greet; "admin"; end
来源：http://vot.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://lrp.epnwcf.com

[G07] 调用父类方法
来源：http://evh.jlsjyb.cn

Py:   super().greet()
来源：http://kjk.xylfe.cn

PHP:  parent::greet();
来源：http://kox.kuanghao11.cn

JS:   super.greet();
来源：http://kfm.jinghuilouyu.cn

TS:   super.greet();
来源：http://zwz.meibo888.top

Java: super.greet();
来源：http://xwd.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hll.svipenyu.cn

Ruby: super
来源：http://vfr.zhiwuduotai.top

C#:   base.Greet();
来源：http://kqs.jqgfzy.top

[G08] 静态方法与属性
来源：http://lix.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rrn.jlsjyb.cn

PHP:  public static function f() {}
来源：http://qjf.gogol.net.cn

JS:   static f() {}
来源：http://dep.hammf.cn

TS:   static f(): void {}
来源：http://goj.gogol.net.cn

Java: static void f() {}
来源：http://aqf.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://unm.zhiwuduotai.top

Ruby: def self.f; end
来源：http://wnc.yuxming.cn

C#:   public static void F() {}
来源：http://spi.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://civ.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://yzw.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://sim.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xqz.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://ifc.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://puw.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://eoe.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lsp.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://ujl.andypj.xyz

[G10] 访问控制
来源：http://jay.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://jxv.tian-w.cn

PHP:  public / protected / private
来源：http://rig.hcnkem.com

JS:   #private 字段；其余公开
来源：http://akr.yueranfly.top

TS:   public / protected / private
来源：http://ucq.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://xxu.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nfp.vehdjk.com

Ruby: public / protected / private
来源：http://dvn.zdqjudy.top

C#:   public / protected / private / internal
来源：http://egu.zdbjq.cn

[G11] getter / setter
来源：http://xaw.xylfe.cn

Py:   @property 与 @x.setter
来源：http://gzk.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zan.gotoacloud.top

JS:   get name() { return this._name; }
来源：http://hov.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://gxs.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://hrt.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://snv.ybcxt.top

Ruby: attr_accessor :name
来源：http://faj.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://gyg.ppjwa.cn

[G12] 对象转字符串
来源：http://wmv.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://lwu.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ylc.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://pxg.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://riw.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://lzm.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://ftd.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://tsu.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://zxr.sjlbkw.cn

[G13] 判断对象类型
来源：http://scb.xziqi.cn

Py:   isinstance(u, User)
来源：http://bpg.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://imk.hnxiangtu.top

JS:   u instanceof User
来源：http://ito.yuxming.cn

TS:   u instanceof User
来源：http://uep.hywenlv.cn

Java: u instanceof User
来源：http://ojy.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uoo.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://chv.ydzc1.top

C#:   u is User
来源：http://jps.zhongyouzk.top

[G14] 数据类 / record
来源：http://jbx.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xlg.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://iag.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://bkd.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://ihg.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://fju.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://pzv.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sap.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://ivg.bbcook.cn

[G15] 枚举
来源：http://ctr.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oje.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wve.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ipw.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eph.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://yea.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lnv.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://kle.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://euk.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://hqm.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ebq.guannengcc.top


<!-- 参考信息 -->