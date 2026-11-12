代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lvg.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://axw.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oin.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qfw.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://smu.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ivr.ydjk.org.cn

Ruby: s.capitalize
来源：http://ifi.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xqn.yueranfly.top

[E18] 模板占位符替换
来源：http://wht.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jsc.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jwt.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hdx.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://hnb.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://moq.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gwa.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kqx.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kdz.316326.xyz

[E19] 多行文本按行拆分
来源：http://udp.cashguo.top

Py:   s.splitlines()
来源：http://ned.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fsj.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://hzj.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://mqy.gotoacloud.top

Java: s.lines().toList()
来源：http://hve.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://isc.gotoacloud.top

Ruby: s.lines
来源：http://xqs.zhijiandao.cn

C#:   s.Split('\n')
来源：http://whf.yonumen.top

[E20] 判断字符串是否为空
来源：http://tgm.shzxlz.cn

Py:   if not s:
来源：http://lfk.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://idd.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wja.aibaodan.cn

TS:   if (s === "") {}
来源：http://hjv.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://nyh.yueranfly.top

Go:   if s == "" {}
来源：http://ihw.hywenlv.cn

Ruby: if s.empty?
来源：http://rru.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yuc.cashguo.top

[E21] 超长截断加省略号
来源：http://ggm.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kpf.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwu.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xcz.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lba.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qjm.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://nts.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://siv.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nmx.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://cci.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://spe.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ygl.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sqd.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sye.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mlv.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kac.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://fqy.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tcl.ehwqpu.com

================================================================================
来源：http://yoh.jinqigfzy.top

F. 文件与目录
来源：http://rse.zhixingplan.top

================================================================================
来源：http://lpl.haohaochexian.top

[F01] 读取整个文件
来源：http://mgd.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gzz.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://wcv.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://djd.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nqy.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tpj.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wvv.xuanzx.com

Ruby: File.read("a.txt")
来源：http://ibx.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://kbo.gzhubu.top

[F02] 逐行读取文件
来源：http://jga.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndo.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://taj.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dnu.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cnu.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eiz.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://azl.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mkc.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hco.tarul.cn

[F03] 写入文件（覆盖）
来源：http://ket.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sbx.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wwx.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ict.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbt.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cak.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bbp.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://jmt.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hov.sufxvd.cn

[F04] 追加写入文件
来源：http://kra.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfk.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dkv.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://apd.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hhx.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dhy.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zrm.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cic.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mea.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://vux.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wib.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://atp.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://xdm.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://tvy.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://laf.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dpb.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://ita.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://vfn.ivvv.top

[F06] 删除文件
来源：http://tgc.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://gue.tian-w.cn

PHP:  unlink("a.txt");
来源：http://etm.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zci.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://uyb.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tzo.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://rna.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://vwj.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://gcl.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://vxw.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://czi.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://frh.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cep.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrd.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ihs.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wlj.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rka.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://apm.uphjek.com

[F08] 遍历目录
来源：http://jba.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cvx.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://efe.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://rlm.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://npf.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vqq.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rsq.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://rdb.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://fxa.nanxuanxn.top

[F09] 获取文件大小
来源：http://mry.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://sct.daxiang520.top

PHP:  filesize("a.txt");
来源：http://dhr.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://wow.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://xfr.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://chj.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kpw.daria6918.cn

Ruby: File.size("a.txt")
来源：http://ufy.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://rwk.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://gkh.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ugx.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eph.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kzk.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://wpg.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nqj.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fbf.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zli.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://msu.ybcxt.top

[F11] 复制与移动文件
来源：http://hvy.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://swr.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iek.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zyl.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dhw.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ezo.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lku.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dgg.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hdo.tianlin.xyz

[F12] CSV 读写
来源：http://opl.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lbe.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cff.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ois.hongshengwenyu.top

TS:   // 同上
来源：http://vai.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ard.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wpr.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://srz.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://izo.tianlin.xyz

================================================================================
来源：http://pkq.sysykeji.top

G. 面向对象
来源：http://hyf.chenjidiqi.icu

================================================================================
来源：http://bxw.shanyushiyangtech.top

[G01] 定义类
来源：http://cnk.fengsongda.top

Py:   class User: pass
来源：http://qnc.jqgufenzy.top

PHP:  class User {}
来源：http://nuf.0kj1m.cn

JS:   class User {}
来源：http://sro.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://tmz.xylfe.cn

Java: class User {}
来源：http://eji.cucudq.cn

Go:   type User struct { Name string }
来源：http://lan.shuidangran.top

Ruby: class User; end
来源：http://egj.fanxiaobao.xyz

C#:   class User {}
来源：http://rtk.tianlin.xyz

[G02] 构造函数
来源：http://vxg.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://big.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://vzx.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://znw.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://vle.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://oor.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ggr.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://psz.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://giu.zhongyouzk.top

[G03] 实例属性
来源：http://zkq.cqqwz.cn

Py:   self.name = "x"
来源：http://vbz.cdnleiting.top

PHP:  public string $name = "x";
来源：http://srr.hcnkem.com

JS:   this.name = "x";
来源：http://rzn.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://spz.chenzaomai.com

Java: private String name;
来源：http://snv.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uks.jianghu66.top

Ruby: @name = "x"
来源：http://zgo.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://asj.haohaochexian.top

[G04] 定义方法
来源：http://jwk.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://iub.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cwg.shuidangran.top

JS:   greet() { return this.name; }
来源：http://qsp.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://kkf.shzxlz.cn

Java: String greet() { return name; }
来源：http://cdw.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cle.jyoumei.cn

Ruby: def greet; @name; end
来源：http://whl.fzhhl.top

C#:   public string Greet() => Name;
来源：http://ujq.jqgufenzy.top

[G05] 继承
来源：http://fts.jiagoushi.top

Py:   class Admin(User): pass
来源：http://sce.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://orq.ehwqpu.com

JS:   class Admin extends User {}
来源：http://qyc.ybcxt.top

TS:   class Admin extends User {}
来源：http://zul.xylfe.cn

Java: class Admin extends User {}
来源：http://oqw.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gjm.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://pdn.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://jel.sxryk.cn

[G06] 重写方法
来源：http://jyu.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://gcs.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mlw.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://gjk.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://fxs.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://hvb.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://akt.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://xno.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://utd.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://izp.yj20258888.top

Py:   super().greet()
来源：http://ihb.fengsongda.top

PHP:  parent::greet();
来源：http://esn.aizwys.cn

JS:   super.greet();
来源：http://dkt.zdqjudy.top

TS:   super.greet();
来源：http://fkm.zhijiandao.cn

Java: super.greet();
来源：http://tkx.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ngb.hongshengwenyu.top

Ruby: super
来源：http://qim.316326.xyz

C#:   base.Greet();
来源：http://yfa.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://xyv.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gkc.xylfe.cn

PHP:  public static function f() {}
来源：http://kun.vqdsnc.cn

JS:   static f() {}
来源：http://hnd.fehbvm.com

TS:   static f(): void {}
来源：http://gla.fanxiaobao.xyz

Java: static void f() {}
来源：http://oew.guowangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://amx.iojbl.cn

Ruby: def self.f; end
来源：http://npt.uphjek.com

C#:   public static void F() {}
来源：http://cvz.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://rei.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://uzx.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vyr.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tpq.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://iar.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://xxy.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://jqe.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qpb.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://yif.zhoulong.xyz

[G10] 访问控制
来源：http://fat.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://src.shzxlz.cn

PHP:  public / protected / private
来源：http://fhd.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://oim.jinghuilouyu.cn

TS:   public / protected / private
来源：http://nsi.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://isq.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zxv.uphjek.com

Ruby: public / protected / private
来源：http://oxc.yj20258888.top

C#:   public / protected / private / internal
来源：http://ouo.vqdsnc.cn

[G11] getter / setter
来源：http://kde.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://box.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jfj.tian-w.cn

JS:   get name() { return this._name; }
来源：http://umq.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://sph.yj20258888.top

Java: public String getName() { return name; }
来源：http://wrb.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nna.tarul.cn

Ruby: attr_accessor :name
来源：http://odp.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://oip.chenlongwang.top

[G12] 对象转字符串
来源：http://xqs.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://ybo.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://omx.yj20258888.top

JS:   toString() { return this.name; }
来源：http://ofz.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://hid.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://cia.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gzb.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://wyj.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://vkp.bjfxy.top

[G13] 判断对象类型
来源：http://ypx.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://nyp.meibo888.top

PHP:  $u instanceof User
来源：http://kht.feifeiyinyue.top

JS:   u instanceof User
来源：http://dki.yonumen.top

TS:   u instanceof User
来源：http://zfx.daria6918.cn

Java: u instanceof User
来源：http://hkx.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xze.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://qcy.zdbjq.cn

C#:   u is User
来源：http://xln.andypj.xyz

[G14] 数据类 / record
来源：http://dny.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fgr.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://qes.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vkl.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://yya.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://zak.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://lng.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjs.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://eap.nwbrower.top

[G15] 枚举
来源：http://iyw.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uhr.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fkd.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://spz.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nyv.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://suc.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xyl.hfpthk.cn


<!-- 参考信息 -->