代发 wailian999

PHP:  number_format(1234567);
来源：http://tdf.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pcd.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xey.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kad.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kly.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://btz.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://rus.jlsjyb.cn

[E17] 首字母大写
来源：http://dnb.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dpm.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wub.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://btb.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rzu.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://znd.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xiz.yfazqb.com

Ruby: s.capitalize
来源：http://ona.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://heu.snrcjt.cn

[E18] 模板占位符替换
来源：http://ulu.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kni.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nkz.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lmr.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dvk.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kbt.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ifd.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pat.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://puw.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://kse.guannengcc.top

Py:   s.splitlines()
来源：http://wmq.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jjx.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://itq.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://hpw.sxryk.cn

Java: s.lines().toList()
来源：http://czb.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://cqu.shuidangran.top

Ruby: s.lines
来源：http://yze.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://lbd.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://zqk.hongshengwenyu.top

Py:   if not s:
来源：http://qwx.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://khr.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zte.hysaishi.cn

TS:   if (s === "") {}
来源：http://tvp.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://rhg.cheryme.top

Go:   if s == "" {}
来源：http://rxm.ydjk.org.cn

Ruby: if s.empty?
来源：http://rit.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://niz.svipenyu.cn

[E21] 超长截断加省略号
来源：http://mvm.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://noo.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://trp.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bke.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjo.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uyl.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://uri.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iuy.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wbk.shuidangran.top

[E22] 字节长度与字符长度
来源：http://lvt.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fad.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uci.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tam.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqn.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rhh.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hbw.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://obx.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ibv.aibaodan.cn

================================================================================
来源：http://xns.yueranfly.top

F. 文件与目录
来源：http://coe.epnwcf.com

================================================================================
来源：http://qjo.nanxuanxn.top

[F01] 读取整个文件
来源：http://jhv.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://acv.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://fvr.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://soa.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nzk.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://utt.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jhs.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://lmj.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://kdq.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://pvs.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mhh.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ndk.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sun.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fon.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bvi.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wre.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dhw.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jmz.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://wzb.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lsn.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ozw.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwk.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eqq.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gha.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wlj.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ork.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tlz.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://kbl.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://enf.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xnm.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://swv.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zka.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sve.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqv.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ooz.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xtk.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://dca.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rgl.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://gbc.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://lhb.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://xei.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ezo.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pyl.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://pmi.uphjek.com

C#:   File.Exists("a.txt")
来源：http://lwo.sysykeji.top

[F06] 删除文件
来源：http://skw.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://ohl.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://sxo.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://avp.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bqg.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ehp.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://qpx.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://ldd.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://fsx.hammf.cn

[F07] 创建目录（含多级）
来源：http://pyp.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://izz.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://grf.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ynm.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nqo.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bzq.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sak.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qkn.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bti.yueranfly.top

[F08] 遍历目录
来源：http://jke.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kvp.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bzx.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://hik.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://ypo.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vls.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://blz.ydzc1.top

Ruby: Dir.children("dir")
来源：http://prn.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://ywe.zycfv.cn

[F09] 获取文件大小
来源：http://qpi.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://fnm.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://ior.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://rjm.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://tfs.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ysm.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qac.vehdjk.com

Ruby: File.size("a.txt")
来源：http://lrz.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://daz.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://aji.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ato.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oau.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ilo.yj20258888.top

TS:   path.extname("a.txt")
来源：http://lqo.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://olu.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qfw.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://doa.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vgx.hammf.cn

[F11] 复制与移动文件
来源：http://cva.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fqj.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lko.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjx.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ouv.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qje.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kxu.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbk.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dup.hesvh.cn

[F12] CSV 读写
来源：http://nao.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rdl.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dnh.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lsy.yj20258888.top

TS:   // 同上
来源：http://qys.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ihf.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://usa.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dlg.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qhw.aibaodan.cn

================================================================================
来源：http://loy.mhx1999.top

G. 面向对象
来源：http://jbi.havefunace.top

================================================================================
来源：http://erq.shzxlz.cn

[G01] 定义类
来源：http://jni.yfazqb.com

Py:   class User: pass
来源：http://vma.sweek.top

PHP:  class User {}
来源：http://aqd.fzhhl.top

JS:   class User {}
来源：http://xhy.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://ukn.gotoacloud.top

Java: class User {}
来源：http://leq.daxiang520.top

Go:   type User struct { Name string }
来源：http://xym.pycfn.com

Ruby: class User; end
来源：http://tua.zhixingplan.top

C#:   class User {}
来源：http://sut.zhongyouzk.top

[G02] 构造函数
来源：http://uwu.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://xuc.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://tum.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://mbb.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://qhw.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://krw.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jlk.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://sqq.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://muk.zhongyouzk.top

[G03] 实例属性
来源：http://llj.yvedp.cn

Py:   self.name = "x"
来源：http://nen.316326.xyz

PHP:  public string $name = "x";
来源：http://eeq.aibaodan.cn

JS:   this.name = "x";
来源：http://fdd.zhixingplan.top

TS:   name: string = "x";
来源：http://biu.sweek.top

Java: private String name;
来源：http://bld.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://esj.hnqzz.top

Ruby: @name = "x"
来源：http://abg.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://zac.shanyushiyangkeji.top

[G04] 定义方法
来源：http://acp.bjfxy.top

Py:   def greet(self): return self.name
来源：http://ceh.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dlo.xuanzx.com

JS:   greet() { return this.name; }
来源：http://rle.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://ovf.jianghu66.top

Java: String greet() { return name; }
来源：http://prl.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rqg.shzxlz.cn

Ruby: def greet; @name; end
来源：http://kpa.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://jlz.fanxiaobao.xyz

[G05] 继承
来源：http://vvt.yj202588.top

Py:   class Admin(User): pass
来源：http://xov.52xcode.cn

PHP:  class Admin extends User {}
来源：http://gir.guannengcc.top

JS:   class Admin extends User {}
来源：http://ruq.uphjek.com

TS:   class Admin extends User {}
来源：http://jby.tianlin.xyz

Java: class Admin extends User {}
来源：http://eml.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tzt.hywenlv.cn

Ruby: class Admin < User; end
来源：http://yoq.hfpthk.cn

C#:   class Admin : User {}
来源：http://wsw.ivvv.top

[G06] 重写方法
来源：http://gho.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://bfo.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://zxb.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://kwa.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://zwb.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://qud.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ggr.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://fil.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://ojs.havefunace.top

[G07] 调用父类方法
来源：http://fqj.bbcook.cn

Py:   super().greet()
来源：http://ktn.xuanzx.com

PHP:  parent::greet();
来源：http://xgu.ydzc1.top

JS:   super.greet();
来源：http://alc.zhoulong.xyz

TS:   super.greet();
来源：http://jbw.epnwcf.com

Java: super.greet();
来源：http://evx.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jhl.aibaodan.cn

Ruby: super
来源：http://ztg.ehwqpu.com

C#:   base.Greet();
来源：http://aja.vehdjk.com

[G08] 静态方法与属性
来源：http://tjq.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qdp.jqgfzy.top

PHP:  public static function f() {}
来源：http://aap.shuidangran.top

JS:   static f() {}
来源：http://ufr.zdqjudy.top

TS:   static f(): void {}
来源：http://xfp.yfazqb.com

Java: static void f() {}
来源：http://vdp.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://afq.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://mwj.316326.xyz

C#:   public static void F() {}
来源：http://qua.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://irv.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://tgk.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://shl.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tuu.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://etm.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://buu.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://atr.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://grt.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://xcr.sufxvd.cn

[G10] 访问控制
来源：http://fvt.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://juj.ehwqpu.com

PHP:  public / protected / private
来源：http://pba.fengsongda.top

JS:   #private 字段；其余公开
来源：http://jhs.shangyingyoupin.top

TS:   public / protected / private
来源：http://oqg.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://zpg.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jth.ehwqpu.com

Ruby: public / protected / private
来源：http://sdq.iojbl.cn

C#:   public / protected / private / internal
来源：http://yiz.cashguo.top

[G11] getter / setter
来源：http://wvx.yj202588.top

Py:   @property 与 @x.setter
来源：http://egt.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jsx.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://ydn.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://syv.yfazqb.com

Java: public String getName() { return name; }
来源：http://jzg.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://viw.aizwys.cn

Ruby: attr_accessor :name
来源：http://esm.daria6918.cn

C#:   public string Name { get; set; }
来源：http://ltk.pycfn.com

[G12] 对象转字符串
来源：http://jwc.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://rgv.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bnc.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://fst.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://xiz.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://jfm.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://ybw.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://xhg.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://vdv.xziqi.cn

[G13] 判断对象类型
来源：http://kcw.tanke756.top

Py:   isinstance(u, User)
来源：http://goj.hysaishi.cn

PHP:  $u instanceof User
来源：http://evr.ctjpmb.com

JS:   u instanceof User
来源：http://zyb.meibo888.top

TS:   u instanceof User
来源：http://msq.hongshengwenyu.top

Java: u instanceof User
来源：http://mzv.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wvs.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://zom.jqgufenzy.top

C#:   u is User
来源：http://djq.snrcjt.cn

[G14] 数据类 / record
来源：http://wxc.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hhk.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://bsu.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://jdj.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://yoh.52xcode.cn

Java: record User(String name, int age) {}
来源：http://hmb.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://bcg.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://orp.epnwcf.com


<!-- 参考信息 -->