代发 wailian999

PHP:  number_format(1234567);
来源：http://vfm.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dtf.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vmz.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://exx.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fcw.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qns.yj20258.top

C#:   1234567.ToString("N0")
来源：http://uvh.fanxiaobao.xyz

[E17] 首字母大写
来源：http://qnm.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kpo.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oex.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tmj.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xha.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hsb.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yyp.hesvh.cn

Ruby: s.capitalize
来源：http://jgu.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oty.hesvh.cn

[E18] 模板占位符替换
来源：http://syo.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://anb.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tfw.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ghc.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bev.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://orb.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ldt.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bom.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qlk.daxiang520.top

[E19] 多行文本按行拆分
来源：http://tyg.aibaodan.cn

Py:   s.splitlines()
来源：http://gyx.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cqe.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://bum.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://evm.nanxinkj.top

Java: s.lines().toList()
来源：http://svh.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://hli.9152youxi.cn

Ruby: s.lines
来源：http://zwv.vehdjk.com

C#:   s.Split('\n')
来源：http://rzd.aizwys.cn

[E20] 判断字符串是否为空
来源：http://vbf.bjfxy.top

Py:   if not s:
来源：http://tdf.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pif.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jlk.zdqjudy.top

TS:   if (s === "") {}
来源：http://nqu.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://nih.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://lpy.kuanghao11.cn

Ruby: if s.empty?
来源：http://bwz.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fyo.shzxlz.cn

[E21] 超长截断加省略号
来源：http://xni.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fak.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dvu.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ntn.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uhy.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rod.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://isw.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ali.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://buy.fehbvm.com

[E22] 字节长度与字符长度
来源：http://zjw.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nrh.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sos.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ssc.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://raf.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rke.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wby.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://kbz.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nvz.tian-w.cn

================================================================================
来源：http://lbb.dashuyun.cn

F. 文件与目录
来源：http://nqi.vehdjk.com

================================================================================
来源：http://oiu.quarkkingdee.top

[F01] 读取整个文件
来源：http://rjr.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hdf.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://ast.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fpt.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jdn.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ajt.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xax.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://hhk.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://nxo.316326.xyz

[F02] 逐行读取文件
来源：http://jth.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yld.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hfv.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xmq.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://utf.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://viu.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qqo.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jja.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ggq.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://upm.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gaa.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mmf.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zbc.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ssa.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xra.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://czi.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://byy.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nkd.xylfe.cn

[F04] 追加写入文件
来源：http://hog.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nmu.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ljv.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://weo.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbn.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cwd.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hno.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vja.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ipq.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://qmn.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wtu.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://pmt.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://kit.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://oln.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://izs.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mpr.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://jnj.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://hyh.ydzc1.top

[F06] 删除文件
来源：http://gjq.yvedp.cn

Py:   os.remove("a.txt")
来源：http://zhf.yongpay.top

PHP:  unlink("a.txt");
来源：http://wli.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://egf.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://eny.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lzb.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://vap.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://vbs.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://ftq.xziqi.cn

[F07] 创建目录（含多级）
来源：http://zcb.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cpk.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xcn.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://adx.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vik.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ply.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zkm.dashuyun.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xvp.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ytw.fengsongda.top

[F08] 遍历目录
来源：http://ssn.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://peb.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fvp.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://tre.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://cko.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ebw.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://geo.smart0.xyz

Ruby: Dir.children("dir")
来源：http://rld.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://eow.ydzc1.top

[F09] 获取文件大小
来源：http://cjx.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://jrn.sysykeji.top

PHP:  filesize("a.txt");
来源：http://qyd.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://fka.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://zjj.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://lmp.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zib.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://kaz.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://wun.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://mjg.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://otf.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tka.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yxu.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://xao.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://msg.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uhu.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nsz.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xfo.jqgufenzy.top

[F11] 复制与移动文件
来源：http://qfo.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fml.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mea.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vtk.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mxk.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nrc.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ead.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sdf.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iaw.xylfe.cn

[F12] CSV 读写
来源：http://anw.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ulr.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cnj.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gst.tianlin.xyz

TS:   // 同上
来源：http://vkq.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hvw.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fru.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ygv.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eam.yueranfly.top

================================================================================
来源：http://iob.guannengcc.top

G. 面向对象
来源：http://vie.meibo888.top

================================================================================
来源：http://msi.ywan-chungtsiang.top

[G01] 定义类
来源：http://kkd.9152youxi.cn

Py:   class User: pass
来源：http://kmi.bjfxy.top

PHP:  class User {}
来源：http://nhc.yj202588.top

JS:   class User {}
来源：http://qyr.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://bms.yanxiufei.cn

Java: class User {}
来源：http://yin.snrcjt.cn

Go:   type User struct { Name string }
来源：http://ffv.redwolf501.top

Ruby: class User; end
来源：http://kvr.jinyuanbaomall.cn

C#:   class User {}
来源：http://vzc.cheryme.top

[G02] 构造函数
来源：http://hev.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://xxr.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://xhm.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://usm.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://ovp.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://ddd.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mys.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://whc.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://nzq.gzhubu.top

[G03] 实例属性
来源：http://qtd.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://mbd.jianghu66.top

PHP:  public string $name = "x";
来源：http://bzt.shuidangran.top

JS:   this.name = "x";
来源：http://swf.gaohongyu789.top

TS:   name: string = "x";
来源：http://uba.haohaochexian.top

Java: private String name;
来源：http://jue.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://liw.dianchejie.cn

Ruby: @name = "x"
来源：http://nea.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://kjv.316326.xyz

[G04] 定义方法
来源：http://vgu.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://jha.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zjn.mhx1999.top

JS:   greet() { return this.name; }
来源：http://ptg.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://ite.jyoumei.cn

Java: String greet() { return name; }
来源：http://rre.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tfe.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://csf.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://ooq.xuetiantiany.cn

[G05] 继承
来源：http://fkf.bjfxy.top

Py:   class Admin(User): pass
来源：http://cia.yonumen.top

PHP:  class Admin extends User {}
来源：http://uyv.bjfxy.top

JS:   class Admin extends User {}
来源：http://udd.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://fnd.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://eyf.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ifp.yfazqb.com

Ruby: class Admin < User; end
来源：http://oim.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://rvu.gzhubu.top

[G06] 重写方法
来源：http://rfe.pycfn.com

Py:   def greet(self): return "admin"
来源：http://tpn.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://kon.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://dbr.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://yuv.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://ovp.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qin.yongpay.top

Ruby: def greet; "admin"; end
来源：http://odo.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://nbk.gotoacloud.top

[G07] 调用父类方法
来源：http://uyz.bbcook.cn

Py:   super().greet()
来源：http://imm.svipenyu.cn

PHP:  parent::greet();
来源：http://vdg.zhiwuduotai.top

JS:   super.greet();
来源：http://box.ctjpmb.com

TS:   super.greet();
来源：http://pax.pengpengdd.cyou

Java: super.greet();
来源：http://ves.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rxl.yj20258888.top

Ruby: super
来源：http://odh.nwbrower.top

C#:   base.Greet();
来源：http://bop.andypj.xyz

[G08] 静态方法与属性
来源：http://fzv.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gmu.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://spt.xinyue.icu

JS:   static f() {}
来源：http://kfe.svipenyu.cn

TS:   static f(): void {}
来源：http://srl.cucudq.cn

Java: static void f() {}
来源：http://onv.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfh.meibo888.top

Ruby: def self.f; end
来源：http://peu.ivvv.top

C#:   public static void F() {}
来源：http://ayw.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://tcc.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://vvw.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://lou.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://bsg.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://qah.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://apa.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://duq.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://css.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://uzq.jinghuilouyu.cn

[G10] 访问控制
来源：http://pvk.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://fur.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://rgy.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://hou.shuidangran.top

TS:   public / protected / private
来源：http://cwn.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://irm.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ltt.yueranfly.top

Ruby: public / protected / private
来源：http://dbo.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://csx.yanxiufei.cn

[G11] getter / setter
来源：http://hpr.yuxming.cn

Py:   @property 与 @x.setter
来源：http://plg.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wpz.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://biv.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://ptx.dianchejie.cn

Java: public String getName() { return name; }
来源：http://dnr.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://itt.jqgfzy.top

Ruby: attr_accessor :name
来源：http://hpn.daxiang520.top

C#:   public string Name { get; set; }
来源：http://qti.sjlbkw.cn

[G12] 对象转字符串
来源：http://ztm.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://pcy.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fnn.zycfv.cn

JS:   toString() { return this.name; }
来源：http://zzf.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://gew.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://mle.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://prn.yj20258888.top

Ruby: def to_s; @name; end
来源：http://hal.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://yuq.aibaodan.cn

[G13] 判断对象类型
来源：http://mbg.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://uea.316326.xyz

PHP:  $u instanceof User
来源：http://dax.hysaishi.cn

JS:   u instanceof User
来源：http://gbf.chenzaomai.com

TS:   u instanceof User
来源：http://urw.hnqzz.top

Java: u instanceof User
来源：http://hva.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ars.tanke756.top

Ruby: u.is_a?(User)
来源：http://nlq.birdmap.top

C#:   u is User
来源：http://jhq.mhx1999.top

[G14] 数据类 / record
来源：http://ulu.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ute.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://ita.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://lrf.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://sqk.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://dqv.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://qkv.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xap.bjfxy.top


<!-- 参考信息 -->