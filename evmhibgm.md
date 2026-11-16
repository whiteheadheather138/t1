代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ryk.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xlw.uphjek.com

Ruby: s.capitalize
来源：http://gzi.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xqb.vehdjk.com

[E18] 模板占位符替换
来源：http://abs.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cxb.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ina.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://igk.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://xpx.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://udd.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfk.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tkd.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kzs.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://tpt.jqgfzy.top

Py:   s.splitlines()
来源：http://szh.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mlf.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://inh.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://orb.kuanghao11.cn

Java: s.lines().toList()
来源：http://uca.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://fwf.hnxiangtu.top

Ruby: s.lines
来源：http://qtc.nanxinkj.top

C#:   s.Split('\n')
来源：http://pdo.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://llm.cdnleiting.top

Py:   if not s:
来源：http://tpx.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vfk.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tht.ybcxt.top

TS:   if (s === "") {}
来源：http://zlz.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://jpj.fengsongda.top

Go:   if s == "" {}
来源：http://qbm.wangshuangyany.cn

Ruby: if s.empty?
来源：http://xvz.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fbj.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://imw.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hyg.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hxo.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbf.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://frf.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pdt.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://dlo.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xeq.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://adr.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://ijl.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rpy.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://slk.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpq.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pnj.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nvj.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vub.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://msj.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nsb.cqqwz.cn

================================================================================
来源：http://cue.yanxiufei.cn

F. 文件与目录
来源：http://tbk.ctjpmb.com

================================================================================
来源：http://psc.yonumen.top

[F01] 读取整个文件
来源：http://dlh.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://roh.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://zur.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eug.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bhm.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ooy.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hjo.meibo888.top

Ruby: File.read("a.txt")
来源：http://vgm.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://cma.shzxlz.cn

[F02] 逐行读取文件
来源：http://wmj.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://thd.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qbf.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zta.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jlj.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://spt.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ela.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://goj.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jdz.316326.xyz

[F03] 写入文件（覆盖）
来源：http://zlz.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xyr.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tlk.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://syo.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jdu.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qpt.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qwg.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://cpo.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://znw.nanxinkj.top

[F04] 追加写入文件
来源：http://umb.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ntr.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pvo.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjd.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://asp.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mfm.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qzk.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dxt.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://drg.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://qwx.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ask.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://rvv.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://qvi.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://qtx.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nax.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kyv.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://faz.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://pxt.zhijiandao.cn

[F06] 删除文件
来源：http://ese.cucudq.cn

Py:   os.remove("a.txt")
来源：http://mmz.xuanzx.com

PHP:  unlink("a.txt");
来源：http://wyi.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://emt.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://fki.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mnh.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://wkw.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://jdt.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://zvb.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://vld.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mvc.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://osl.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kml.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myw.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rip.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gir.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://frk.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iao.hammf.cn

[F08] 遍历目录
来源：http://fvd.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yiy.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ghq.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://awz.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://sjz.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gum.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ugt.vehdjk.com

Ruby: Dir.children("dir")
来源：http://fef.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://awb.sjlbkw.cn

[F09] 获取文件大小
来源：http://vhl.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://dou.c1oappe.top

PHP:  filesize("a.txt");
来源：http://fmi.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://gbr.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://wis.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://sat.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kbc.bjfxy.top

Ruby: File.size("a.txt")
来源：http://ngu.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://ixb.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://awt.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ixs.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwt.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://epb.hesvh.cn

TS:   path.extname("a.txt")
来源：http://jjz.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uun.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xjn.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tym.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://meh.guowangkeji.top

[F11] 复制与移动文件
来源：http://kln.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://udy.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fgt.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blt.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://otl.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pye.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdf.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jbk.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ifb.9152youxi.cn

[F12] CSV 读写
来源：http://igk.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rew.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nim.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pyl.hnqzz.top

TS:   // 同上
来源：http://kwy.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zyo.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yjy.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ugx.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tzs.vqdsnc.cn

================================================================================
来源：http://kof.hongshengwenyu.top

G. 面向对象
来源：http://mvz.yanxiufei.cn

================================================================================
来源：http://ybp.316326.xyz

[G01] 定义类
来源：http://brw.tanke756.top

Py:   class User: pass
来源：http://sem.chenlongwang.top

PHP:  class User {}
来源：http://wmz.shanyushiyangtech.top

JS:   class User {}
来源：http://mzu.yonumen.top

TS:   class User { name: string = ""; }
来源：http://sum.fktsv.cn

Java: class User {}
来源：http://sbk.52xcode.cn

Go:   type User struct { Name string }
来源：http://gcg.jqgufenzy.top

Ruby: class User; end
来源：http://tmp.fengsongda.top

C#:   class User {}
来源：http://fus.cucudq.cn

[G02] 构造函数
来源：http://ehn.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://tnu.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://xwx.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://qei.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://qfh.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://jwq.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zsl.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://utf.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://vdl.zdbjq.cn

[G03] 实例属性
来源：http://jgb.cheryme.top

Py:   self.name = "x"
来源：http://phr.guannengcc.top

PHP:  public string $name = "x";
来源：http://tjs.daxiang520.top

JS:   this.name = "x";
来源：http://xej.redwolf501.top

TS:   name: string = "x";
来源：http://xxi.shzxlz.cn

Java: private String name;
来源：http://ixz.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ttx.52xcode.cn

Ruby: @name = "x"
来源：http://qjp.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://bbt.tianlin.xyz

[G04] 定义方法
来源：http://ser.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://jol.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://inp.nwbrower.top

JS:   greet() { return this.name; }
来源：http://stt.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://psa.hfpthk.cn

Java: String greet() { return name; }
来源：http://vso.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cas.yueranfly.top

Ruby: def greet; @name; end
来源：http://tlm.cucudq.cn

C#:   public string Greet() => Name;
来源：http://adx.smart0.xyz

[G05] 继承
来源：http://ksq.gzhubu.top

Py:   class Admin(User): pass
来源：http://sqd.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://njb.yfazqb.com

JS:   class Admin extends User {}
来源：http://isf.yuxming.cn

TS:   class Admin extends User {}
来源：http://bdr.cheryme.top

Java: class Admin extends User {}
来源：http://lof.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://apu.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://oco.jqgufenzy.top

C#:   class Admin : User {}
来源：http://nyb.guannengcc.top

[G06] 重写方法
来源：http://dhp.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://gtf.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nhq.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://eha.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://iur.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://ndj.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hvw.tanke756.top

Ruby: def greet; "admin"; end
来源：http://ink.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://ppa.shangyingyoupin.top

[G07] 调用父类方法
来源：http://hlp.zdbjq.cn

Py:   super().greet()
来源：http://kds.hnqzz.top

PHP:  parent::greet();
来源：http://vej.tanke756.top

JS:   super.greet();
来源：http://dxd.tarul.cn

TS:   super.greet();
来源：http://nss.zhengqikj.top

Java: super.greet();
来源：http://yhq.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://smp.9152youxi.cn

Ruby: super
来源：http://jyq.birdmap.top

C#:   base.Greet();
来源：http://ztl.hammf.cn

[G08] 静态方法与属性
来源：http://owo.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tuf.jlsjyb.cn

PHP:  public static function f() {}
来源：http://uvg.jinqigfzy.top

JS:   static f() {}
来源：http://uon.vehdjk.com

TS:   static f(): void {}
来源：http://ybq.zhixingplan.top

Java: static void f() {}
来源：http://ibw.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nbw.0kj1m.cn

Ruby: def self.f; end
来源：http://vhq.shuidangran.top

C#:   public static void F() {}
来源：http://zfu.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://uuy.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://tmx.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://yqb.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lqg.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://qqu.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://vnq.jinqigufen.top

Go:   type Shape interface { Area() float64 }
来源：http://jie.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yzw.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://sei.ivvv.top

[G10] 访问控制
来源：http://ixi.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://eyh.ybcxt.top

PHP:  public / protected / private
来源：http://edc.cashguo.top

JS:   #private 字段；其余公开
来源：http://rqj.jqgufenzy.top

TS:   public / protected / private
来源：http://ngw.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://cij.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qfr.shzxlz.cn

Ruby: public / protected / private
来源：http://mza.fzhhl.top

C#:   public / protected / private / internal
来源：http://sbq.cdnleiting.top

[G11] getter / setter
来源：http://ach.316326.xyz

Py:   @property 与 @x.setter
来源：http://stu.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cuf.c1oappe.top

JS:   get name() { return this._name; }
来源：http://tnj.mhx1999.top

TS:   get name(): string { return this._name; }
来源：http://ovo.epnwcf.com

Java: public String getName() { return name; }
来源：http://jri.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kwh.hcnkem.com

Ruby: attr_accessor :name
来源：http://pop.meibo888.top

C#:   public string Name { get; set; }
来源：http://ozn.dashuyun.cn

[G12] 对象转字符串
来源：http://roc.yj202588.top

Py:   def __str__(self): return self.name
来源：http://zzm.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kjt.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://asw.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://whh.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://hyq.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://klo.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://nld.cheryme.top

C#:   public override string ToString() => Name;
来源：http://qtq.pengpengdd.cyou

[G13] 判断对象类型
来源：http://qmu.birdmap.top

Py:   isinstance(u, User)
来源：http://vyn.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://ltr.iojbl.cn

JS:   u instanceof User
来源：http://lfe.snrcjt.cn

TS:   u instanceof User
来源：http://ooy.ctjpmb.com

Java: u instanceof User
来源：http://ghs.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cwj.yj20258888.top

Ruby: u.is_a?(User)
来源：http://mvm.316326.xyz

C#:   u is User
来源：http://jxs.smart0.xyz

[G14] 数据类 / record
来源：http://taj.ctjpmb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://knf.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://umn.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://wjr.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://qvz.yueranfly.top

Java: record User(String name, int age) {}
来源：http://btm.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://sov.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mmu.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://hxl.jqgfzy.top

[G15] 枚举
来源：http://hjo.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vnn.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wkx.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lsz.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bep.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://msp.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zdj.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://mxy.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dlv.havefunace.top

[G16] 对象转数组 / 字典
来源：http://awx.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ygo.wangdashe.top


<!-- 参考信息 -->