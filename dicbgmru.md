代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ata.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zbz.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://mwy.yueranfly.top

[E17] 首字母大写
来源：http://mcr.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ngm.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qqq.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://squ.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pfn.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tex.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ten.feifeiyinyue.top

Ruby: s.capitalize
来源：http://qiu.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yfl.cashguo.top

[E18] 模板占位符替换
来源：http://srx.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://clb.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eea.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://adk.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bvu.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://evx.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bsm.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wab.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nkf.daria6918.cn

[E19] 多行文本按行拆分
来源：http://lwq.uphjek.com

Py:   s.splitlines()
来源：http://wme.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hrw.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://egm.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://fdo.xuetiantiany.cn

Java: s.lines().toList()
来源：http://kph.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://jck.jqgufenzy.top

Ruby: s.lines
来源：http://hfj.c1oappe.top

C#:   s.Split('\n')
来源：http://pbv.hammf.cn

[E20] 判断字符串是否为空
来源：http://euz.tianlin.xyz

Py:   if not s:
来源：http://emq.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wdz.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kwq.hnqzz.top

TS:   if (s === "") {}
来源：http://scl.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://hmx.nanxinkj.top

Go:   if s == "" {}
来源：http://xhd.hywenlv.cn

Ruby: if s.empty?
来源：http://ccw.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blw.uphjek.com

[E21] 超长截断加省略号
来源：http://pmi.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mwg.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bam.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jpz.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrk.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gfu.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://bts.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwt.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xdz.fehbvm.com

[E22] 字节长度与字符长度
来源：http://xxk.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bfk.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nhq.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pgj.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lgl.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qho.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kid.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://vpv.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://luq.xylfe.cn

================================================================================
来源：http://qci.andypj.xyz

F. 文件与目录
来源：http://mmw.zhongyouzk.top

================================================================================
来源：http://tgf.cucudq.cn

[F01] 读取整个文件
来源：http://koy.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zuf.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://umd.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hby.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wqy.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://was.xingfuxueyuan.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vjt.xziqi.cn

Ruby: File.read("a.txt")
来源：http://awa.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://cbl.yangfankeji.com

[F02] 逐行读取文件
来源：http://kgm.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wxz.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrm.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hgt.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qsq.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://chj.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://chf.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vvi.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uvz.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://svg.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://otj.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kdq.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zmk.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://olw.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ttx.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wuj.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://aei.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oky.wangshuangyany.cn

[F04] 追加写入文件
来源：http://gew.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bnu.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nuv.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sck.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gno.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nbz.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ujz.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hog.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pip.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://ioz.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zrq.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://qnk.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://hqs.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://pay.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vqr.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vmb.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://mdn.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://wmq.yfazqb.com

[F06] 删除文件
来源：http://ztt.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://vjp.sweek.top

PHP:  unlink("a.txt");
来源：http://zrm.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://mnz.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pkq.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qby.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://yaq.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://zsg.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://gqb.ivvv.top

[F07] 创建目录（含多级）
来源：http://hqu.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://daj.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lhq.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lbn.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ctn.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ybh.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfu.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uat.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlp.chenzaomai.com

[F08] 遍历目录
来源：http://div.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mkd.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nkv.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://mrz.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://lvc.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bmi.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://asx.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://lqc.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://rrt.hammf.cn

[F09] 获取文件大小
来源：http://eom.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://qdv.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://ssu.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://nrg.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://whg.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://osp.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aoj.fengsongda.top

Ruby: File.size("a.txt")
来源：http://tex.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://cqn.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://vll.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzi.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iwf.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pzc.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://mns.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qnp.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://akf.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yay.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rtl.hesvh.cn

[F11] 复制与移动文件
来源：http://zlv.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vfw.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gwd.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aer.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://onb.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wor.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ice.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ozs.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oop.ybcxt.top

[F12] CSV 读写
来源：http://mfb.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nqu.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tde.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sgk.yj20258888.top

TS:   // 同上
来源：http://lfc.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rsz.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vbb.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bnq.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://guu.zhongyouzk.top

================================================================================
来源：http://grq.kuanghao11.cn

G. 面向对象
来源：http://rnv.nanxinkj.top

================================================================================
来源：http://hmj.fzhhl.top

[G01] 定义类
来源：http://wbv.ydzc1.top

Py:   class User: pass
来源：http://oxc.hnxiangtu.top

PHP:  class User {}
来源：http://lja.smart0.xyz

JS:   class User {}
来源：http://cot.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://tpc.ehwqpu.com

Java: class User {}
来源：http://ipc.smart0.xyz

Go:   type User struct { Name string }
来源：http://mel.ydzc1.top

Ruby: class User; end
来源：http://rdz.zdqjudy.top

C#:   class User {}
来源：http://pqj.chenlongwang.top

[G02] 构造函数
来源：http://yor.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://tap.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://vml.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://brg.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://sei.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://vlu.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pcx.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://wsg.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://pjx.fzhhl.top

[G03] 实例属性
来源：http://hvy.yuxming.cn

Py:   self.name = "x"
来源：http://ckx.tarul.cn

PHP:  public string $name = "x";
来源：http://btx.xinyue.icu

JS:   this.name = "x";
来源：http://ydl.jianghu66.top

TS:   name: string = "x";
来源：http://wuw.nanxuanxn.top

Java: private String name;
来源：http://gpd.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://myv.snrcjt.cn

Ruby: @name = "x"
来源：http://gmn.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://inc.yj20258888.top

[G04] 定义方法
来源：http://otv.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://gtv.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zme.yongpay.top

JS:   greet() { return this.name; }
来源：http://rcn.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://kzy.yj20258888.top

Java: String greet() { return name; }
来源：http://qyz.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://lvq.pycfn.com

Ruby: def greet; @name; end
来源：http://hzo.yj20258.top

C#:   public string Greet() => Name;
来源：http://kib.sjlbkw.cn

[G05] 继承
来源：http://opt.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://kqs.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://adi.yfazqb.com

JS:   class Admin extends User {}
来源：http://mxt.haohaochexian.top

TS:   class Admin extends User {}
来源：http://dkq.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://uxq.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wpm.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://esl.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://ghg.yanxiufei.cn

[G06] 重写方法
来源：http://vvd.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://tws.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ujx.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://ywd.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://pph.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://qbg.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sgv.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://vsk.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://dgf.jqgfzy.top

[G07] 调用父类方法
来源：http://gii.ydzc1.top

Py:   super().greet()
来源：http://jsh.yongpay.top

PHP:  parent::greet();
来源：http://hdw.shanyushiyangkeji.top

JS:   super.greet();
来源：http://sjz.sweek.top

TS:   super.greet();
来源：http://ttc.guowangkeji.top

Java: super.greet();
来源：http://rug.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wci.andypj.xyz

Ruby: super
来源：http://zhx.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://ski.zhoulong.xyz

[G08] 静态方法与属性
来源：http://jnz.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yjd.jyoumei.cn

PHP:  public static function f() {}
来源：http://hjb.yuxming.cn

JS:   static f() {}
来源：http://dgl.zdqjudy.top

TS:   static f(): void {}
来源：http://nhd.shanyushiyangtech.top

Java: static void f() {}
来源：http://icu.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://swq.hesvh.cn

Ruby: def self.f; end
来源：http://bmy.jinqigfzy.top

C#:   public static void F() {}
来源：http://sex.xylfe.cn

[G09] 接口 / 抽象类
来源：http://qjg.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://bld.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://aya.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kga.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://jhb.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://ihp.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://hhf.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pyk.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://yqj.cucudq.cn

[G10] 访问控制
来源：http://sec.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://miw.hongshengwenyu.top

PHP:  public / protected / private
来源：http://fyi.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://gcn.bjfxy.top

TS:   public / protected / private
来源：http://gfa.ivvv.top

Java: public / protected / private / 默认包级
来源：http://zax.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zvv.wangdashe.top

Ruby: public / protected / private
来源：http://udo.jqgfzy.top

C#:   public / protected / private / internal
来源：http://fuo.uphjek.com

[G11] getter / setter
来源：http://pxt.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://mie.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gol.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://ajq.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://fdt.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://zim.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ixj.fzhhl.top

Ruby: attr_accessor :name
来源：http://iac.cheryme.top

C#:   public string Name { get; set; }
来源：http://ujz.hnqzz.top

[G12] 对象转字符串
来源：http://vko.uphjek.com

Py:   def __str__(self): return self.name
来源：http://ivb.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://udh.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://whg.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://vga.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://qny.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pdk.birdmap.top

Ruby: def to_s; @name; end
来源：http://wqu.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://nvx.jyoumei.cn

[G13] 判断对象类型
来源：http://tho.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://dku.0kj1m.cn

PHP:  $u instanceof User
来源：http://egh.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://ksq.hongshengwenyu.top

TS:   u instanceof User
来源：http://nvw.yangfankeji.com

Java: u instanceof User
来源：http://upn.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eel.redwolf501.top

Ruby: u.is_a?(User)
来源：http://zvv.sjlbkw.cn

C#:   u is User
来源：http://cjj.sxryk.cn

[G14] 数据类 / record
来源：http://qus.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vcf.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://zfx.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oew.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://dhl.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://fvk.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://tmf.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oii.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://drh.sufxvd.cn

[G15] 枚举
来源：http://lhl.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://edp.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kob.zycfv.cn


<!-- 参考信息 -->