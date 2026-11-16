代发 wailian999

[E18] 模板占位符替换
来源：http://bcs.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://efz.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://opl.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dzi.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xsa.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vda.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mhg.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://reg.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://acf.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://hdt.mhx1999.top

Py:   s.splitlines()
来源：http://ggd.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://igf.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://epe.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://jyj.jqgfzy.top

Java: s.lines().toList()
来源：http://lmk.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://mli.yfazqb.com

Ruby: s.lines
来源：http://xpo.jqgufenzy.top

C#:   s.Split('\n')
来源：http://bgz.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://cjw.zhongyouzk.top

Py:   if not s:
来源：http://mxh.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wlu.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jrd.hnxiangtu.top

TS:   if (s === "") {}
来源：http://fcn.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://hpj.meibo888.top

Go:   if s == "" {}
来源：http://qyu.sysykeji.top

Ruby: if s.empty?
来源：http://stz.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://syp.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://yal.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xfp.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcf.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iob.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pcl.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sap.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://xva.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qyb.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://par.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://sqc.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dmq.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wdj.hcnkem.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fma.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjx.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cyt.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qwi.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://nga.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xyp.zhongyouzk.top

================================================================================
来源：http://lcg.daria6918.cn

F. 文件与目录
来源：http://fuy.daria6918.cn

================================================================================
来源：http://hro.chenjidiqi.icu

[F01] 读取整个文件
来源：http://mry.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mef.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://oqo.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mwv.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oat.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jhr.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://obh.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://maz.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://rzm.uphjek.com

[F02] 逐行读取文件
来源：http://cnr.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://njq.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uro.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oyu.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gjn.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tds.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gno.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ihm.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hgc.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://prr.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qyz.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://avx.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hrh.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ciu.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xiu.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iqt.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://qvv.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kxr.jqgfzy.top

[F04] 追加写入文件
来源：http://jhp.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hak.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qsp.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aej.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kxw.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fan.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://raa.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fhx.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iiq.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://czo.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjm.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://iqn.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://sds.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://iwx.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ate.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yck.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://grm.cheryme.top

C#:   File.Exists("a.txt")
来源：http://nrm.yj20258.top

[F06] 删除文件
来源：http://rts.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://ldc.c1oappe.top

PHP:  unlink("a.txt");
来源：http://bsc.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://szw.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mdv.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rxt.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://utq.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://wau.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://lkj.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://lqr.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mga.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://drq.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pea.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dck.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mqv.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hcj.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cyz.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://osn.iojbl.cn

[F08] 遍历目录
来源：http://nsp.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xdy.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bjv.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://jnb.sweek.top

TS:   fs.readdirSync("dir")
来源：http://pab.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blv.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xze.sysykeji.top

Ruby: Dir.children("dir")
来源：http://ztd.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://wev.zdqjudy.top

[F09] 获取文件大小
来源：http://aml.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://gux.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://eht.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://mci.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://beb.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://bpe.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bri.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://ctz.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://qty.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://usw.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ldy.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fip.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://shv.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://qzp.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mli.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lek.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kap.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mos.gotoacloud.top

[F11] 复制与移动文件
来源：http://vdv.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qmu.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wes.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvf.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ooj.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ico.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pau.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iim.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yfc.zhongyouzk.top

[F12] CSV 读写
来源：http://vcc.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mpv.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://irc.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ekf.hfpthk.cn

TS:   // 同上
来源：http://gaq.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bha.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mga.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pbn.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bwj.bjfxy.top

================================================================================
来源：http://ica.redwolf501.top

G. 面向对象
来源：http://fgf.kuanghao11.cn

================================================================================
来源：http://ywq.0kj1m.cn

[G01] 定义类
来源：http://iwf.andypj.xyz

Py:   class User: pass
来源：http://ljk.sjlbkw.cn

PHP:  class User {}
来源：http://vie.0kj1m.cn

JS:   class User {}
来源：http://qqw.tanke756.top

TS:   class User { name: string = ""; }
来源：http://zyc.sxryk.cn

Java: class User {}
来源：http://lbr.hammf.cn

Go:   type User struct { Name string }
来源：http://xhu.cucudq.cn

Ruby: class User; end
来源：http://bys.ybcxt.top

C#:   class User {}
来源：http://rrg.yj20258888.top

[G02] 构造函数
来源：http://sno.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://bqn.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://rrl.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://kzx.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://cpj.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://efa.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://son.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://sah.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://ttn.jlsjyb.cn

[G03] 实例属性
来源：http://knb.hongshengwenyu.top

Py:   self.name = "x"
来源：http://adl.sysykeji.top

PHP:  public string $name = "x";
来源：http://lwm.hcnkem.com

JS:   this.name = "x";
来源：http://gdm.jiagoushi.top

TS:   name: string = "x";
来源：http://xkx.yanxiufei.cn

Java: private String name;
来源：http://ypv.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jbl.yj20258888.top

Ruby: @name = "x"
来源：http://mgw.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://kbs.tianlin.xyz

[G04] 定义方法
来源：http://djy.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://chf.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://nyv.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://mng.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://gew.sjlbkw.cn

Java: String greet() { return name; }
来源：http://ufk.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://seo.andypj.xyz

Ruby: def greet; @name; end
来源：http://lys.hesvh.cn

C#:   public string Greet() => Name;
来源：http://knf.snrcjt.cn

[G05] 继承
来源：http://qna.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://yjb.guannengcc.top

PHP:  class Admin extends User {}
来源：http://cax.redwolf501.top

JS:   class Admin extends User {}
来源：http://mdz.ehwqpu.com

TS:   class Admin extends User {}
来源：http://kei.c1oappe.top

Java: class Admin extends User {}
来源：http://xsu.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://udf.yvedp.cn

Ruby: class Admin < User; end
来源：http://slu.wangdashe.top

C#:   class Admin : User {}
来源：http://yem.gaohongyu789.top

[G06] 重写方法
来源：http://frd.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://bxe.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tkw.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://qvm.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://pnp.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://mpo.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xog.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://djt.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://efo.guannengcc.top

[G07] 调用父类方法
来源：http://gzk.bbcook.cn

Py:   super().greet()
来源：http://yfd.ydjk.org.cn

PHP:  parent::greet();
来源：http://rug.jinyuanbaomall.cn

JS:   super.greet();
来源：http://xsw.ybcxt.top

TS:   super.greet();
来源：http://eic.guowangkeji.top

Java: super.greet();
来源：http://nbh.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hvf.wangshuangyany.cn

Ruby: super
来源：http://ysk.gotoacloud.top

C#:   base.Greet();
来源：http://fda.zdbjq.cn

[G08] 静态方法与属性
来源：http://teb.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yfn.zhoulong.xyz

PHP:  public static function f() {}
来源：http://hsw.jinghuilouyu.cn

JS:   static f() {}
来源：http://ngj.cdnleiting.top

TS:   static f(): void {}
来源：http://tww.52xcode.cn

Java: static void f() {}
来源：http://uvh.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vru.kuanghao11.cn

Ruby: def self.f; end
来源：http://yii.chenlongwang.top

C#:   public static void F() {}
来源：http://rsh.xylfe.cn

[G09] 接口 / 抽象类
来源：http://uuz.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://qgm.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hst.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gxo.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://gfx.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://dnh.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://rjo.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://inx.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://asx.tanke756.top

[G10] 访问控制
来源：http://uqj.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ilq.andypj.xyz

PHP:  public / protected / private
来源：http://lfc.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://aen.daxiang520.top

TS:   public / protected / private
来源：http://als.yonumen.top

Java: public / protected / private / 默认包级
来源：http://awr.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kmx.9152youxi.cn

Ruby: public / protected / private
来源：http://xqq.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://itv.xziqi.cn

[G11] getter / setter
来源：http://iqi.guannengcc.top

Py:   @property 与 @x.setter
来源：http://qjb.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pft.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://hgj.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://igd.xziqi.cn

Java: public String getName() { return name; }
来源：http://upt.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://knx.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://ouo.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://fae.sweek.top

[G12] 对象转字符串
来源：http://vfb.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://xuv.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wkq.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://nnr.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://nsr.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://whx.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://nqd.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://fzk.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://fkv.fzhhl.top

[G13] 判断对象类型
来源：http://ysu.yuanzhike.top

Py:   isinstance(u, User)
来源：http://ugh.hfpthk.cn

PHP:  $u instanceof User
来源：http://vmc.yanxiufei.cn

JS:   u instanceof User
来源：http://apq.quarkkingdee.top

TS:   u instanceof User
来源：http://qod.zdbjq.cn

Java: u instanceof User
来源：http://got.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://hyz.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://nnz.xuanzx.com

C#:   u is User
来源：http://tkw.yj202588.top

[G14] 数据类 / record
来源：http://amw.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ecm.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://bhd.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://cpw.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://jcg.tarul.cn

Java: record User(String name, int age) {}
来源：http://vng.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://pkh.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ugj.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://dxt.xuanzx.com

[G15] 枚举
来源：http://hnm.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vuq.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nvw.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lpy.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sbr.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://ilf.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rla.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://zai.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hte.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://qxb.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iao.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://wgp.hysaishi.cn

JS:   Object.entries(obj)
来源：http://wnd.zhengqikj.top

TS:   Object.entries(obj)
来源：http://pxc.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zhj.zhengqikj.top


<!-- 参考信息 -->