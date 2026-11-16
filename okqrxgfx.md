代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nvf.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://iep.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ged.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eec.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pus.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://thm.yangfankeji.com

Ruby: s.capitalize
来源：http://mpa.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fwj.nanxinkj.top

[E18] 模板占位符替换
来源：http://yvr.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uyq.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vhg.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://gqk.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gky.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sfn.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dph.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wfa.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wab.yueranfly.top

[E19] 多行文本按行拆分
来源：http://rxh.tarul.cn

Py:   s.splitlines()
来源：http://okr.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ffs.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://cux.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://toq.tianlin.xyz

Java: s.lines().toList()
来源：http://lwd.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://flc.meibo888.top

Ruby: s.lines
来源：http://qez.yj20258.top

C#:   s.Split('\n')
来源：http://orc.havefunace.top

[E20] 判断字符串是否为空
来源：http://kyb.tarul.cn

Py:   if not s:
来源：http://zvz.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sos.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xlx.hesvh.cn

TS:   if (s === "") {}
来源：http://axy.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://yjv.yueranfly.top

Go:   if s == "" {}
来源：http://rcd.xziqi.cn

Ruby: if s.empty?
来源：http://ecu.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ufc.0kj1m.cn

[E21] 超长截断加省略号
来源：http://zqr.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qvx.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nkf.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rbc.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rqe.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tmq.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://ytd.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ido.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uan.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://ftl.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://djo.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://goi.jlsjyb.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mrq.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bnh.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iro.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mkd.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://uxj.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zbf.c1oappe.top

================================================================================
来源：http://tgq.shangyingyoupin.top

F. 文件与目录
来源：http://khq.yuanzhike.top

================================================================================
来源：http://guk.daria6918.cn

[F01] 读取整个文件
来源：http://ign.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ogo.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://ykb.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rse.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://awb.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xes.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rvh.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://pmn.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://fwp.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://dlu.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dxy.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ppz.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywt.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uby.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wlr.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ive.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bkx.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://osa.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://gln.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lhi.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rmt.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yxu.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffq.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wuy.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tzb.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://pir.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rpn.uphjek.com

[F04] 追加写入文件
来源：http://kly.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://srj.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tdo.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lps.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azt.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yjg.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xnq.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wqc.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xev.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://vtr.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://owo.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://kdl.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://gwn.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://fbt.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qjh.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sho.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://gyf.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://nei.uphjek.com

[F06] 删除文件
来源：http://qyx.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://fem.fehbvm.com

PHP:  unlink("a.txt");
来源：http://dqu.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fok.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ghr.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rgd.316326.xyz

Go:   os.Remove("a.txt")
来源：http://wef.cheryme.top

Ruby: File.delete("a.txt")
来源：http://tpt.yonumen.top

C#:   File.Delete("a.txt");
来源：http://noe.hcnkem.com

[F07] 创建目录（含多级）
来源：http://yci.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gyk.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uha.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iog.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://huu.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yxa.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aog.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gtl.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://izm.wangdashe.top

[F08] 遍历目录
来源：http://gpk.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://izt.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oyg.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://mzl.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://ltt.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rdj.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://riv.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://gmf.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://eiy.tarul.cn

[F09] 获取文件大小
来源：http://nch.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://apv.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://sog.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://wvn.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://mha.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://pcx.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://adr.bjfxy.top

Ruby: File.size("a.txt")
来源：http://lvy.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://mwu.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://bsj.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cjg.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://avc.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ona.yfazqb.com

TS:   path.extname("a.txt")
来源：http://cec.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oea.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gfp.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zvd.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://muo.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://bbv.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oag.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mky.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kre.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dft.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://njm.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tdk.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jxh.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bbd.jqgfzy.top

[F12] CSV 读写
来源：http://gpd.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://via.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zek.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fta.shuidangran.top

TS:   // 同上
来源：http://bhu.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://abj.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ebp.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xks.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hpp.bjfxy.top

================================================================================
来源：http://uqi.daxiang520.top

G. 面向对象
来源：http://ast.tarul.cn

================================================================================
来源：http://koa.yanxiufei.cn

[G01] 定义类
来源：http://rhf.tanke756.top

Py:   class User: pass
来源：http://qrb.shangyingyoupin.top

PHP:  class User {}
来源：http://cjc.zhoulong.xyz

JS:   class User {}
来源：http://xto.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://jxe.chenjidiqi.icu

Java: class User {}
来源：http://lzr.meibo888.top

Go:   type User struct { Name string }
来源：http://jer.wangdashe.top

Ruby: class User; end
来源：http://zgp.52xcode.cn

C#:   class User {}
来源：http://vvy.feifeiyinyue.top

[G02] 构造函数
来源：http://jal.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://cji.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://zru.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://nrm.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://jxp.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://apn.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yfp.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://sbg.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://xlk.zdqjudy.top

[G03] 实例属性
来源：http://ibc.cdnleiting.top

Py:   self.name = "x"
来源：http://mox.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://nym.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://oza.jlsjyb.cn

TS:   name: string = "x";
来源：http://vbp.yongpay.top

Java: private String name;
来源：http://kfg.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sbk.jlsjyb.cn

Ruby: @name = "x"
来源：http://bkk.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://wqi.chenlongwang.top

[G04] 定义方法
来源：http://oxs.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://qdl.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kpy.xinyue.icu

JS:   greet() { return this.name; }
来源：http://ewy.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://tvd.svipenyu.cn

Java: String greet() { return name; }
来源：http://xmm.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sfb.jqgfzy.top

Ruby: def greet; @name; end
来源：http://ftp.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://rif.gotoacloud.top

[G05] 继承
来源：http://xlz.yj20258.top

Py:   class Admin(User): pass
来源：http://fuv.ybcxt.top

PHP:  class Admin extends User {}
来源：http://xjg.jqgfzy.top

JS:   class Admin extends User {}
来源：http://zvc.birdmap.top

TS:   class Admin extends User {}
来源：http://xuh.ehwqpu.com

Java: class Admin extends User {}
来源：http://ojz.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nlr.fehbvm.com

Ruby: class Admin < User; end
来源：http://iqk.birdmap.top

C#:   class Admin : User {}
来源：http://nlx.hammf.cn

[G06] 重写方法
来源：http://lqd.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://nzp.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pps.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://jlu.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://euw.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://noh.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tzf.havefunace.top

Ruby: def greet; "admin"; end
来源：http://fxm.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://umu.gaohongyu789.top

[G07] 调用父类方法
来源：http://lbr.nanxinkj.top

Py:   super().greet()
来源：http://sjm.tanke756.top

PHP:  parent::greet();
来源：http://vub.ywan-chungtsiang.top

JS:   super.greet();
来源：http://ufn.cucudq.cn

TS:   super.greet();
来源：http://auh.aibaodan.cn

Java: super.greet();
来源：http://qhh.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ufw.xinyue.icu

Ruby: super
来源：http://bwv.daria6918.cn

C#:   base.Greet();
来源：http://pki.hesvh.cn

[G08] 静态方法与属性
来源：http://bms.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nhx.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://apd.tianlin.xyz

JS:   static f() {}
来源：http://gcd.9152youxi.cn

TS:   static f(): void {}
来源：http://brv.fktsv.cn

Java: static void f() {}
来源：http://ujk.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xme.jiagoushi.top

Ruby: def self.f; end
来源：http://zkg.yj202588.top

C#:   public static void F() {}
来源：http://oqr.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://qtl.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://hrj.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xnr.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://wfk.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://brs.gzhubu.top

Java: interface Shape { double area(); }
来源：http://yea.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://lta.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ycv.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://ehc.yanxiufei.cn

[G10] 访问控制
来源：http://xld.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://hle.zycfv.cn

PHP:  public / protected / private
来源：http://jxg.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://kih.zhijiandao.cn

TS:   public / protected / private
来源：http://vjs.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://cyn.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fvg.ybcxt.top

Ruby: public / protected / private
来源：http://olz.jinqigufen.top

C#:   public / protected / private / internal
来源：http://qhs.zhixingplan.top

[G11] getter / setter
来源：http://srv.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://rsb.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wjl.zycfv.cn

JS:   get name() { return this._name; }
来源：http://gnj.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://ost.guowangkeji.top

Java: public String getName() { return name; }
来源：http://bxc.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cja.mhx1999.top

Ruby: attr_accessor :name
来源：http://gzf.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://wbx.yj20258.top

[G12] 对象转字符串
来源：http://ade.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://tkm.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xmp.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://hyj.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://abu.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://dbi.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://xow.pycfn.com

Ruby: def to_s; @name; end
来源：http://iol.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://ine.zdbjq.cn

[G13] 判断对象类型
来源：http://caw.uphjek.com

Py:   isinstance(u, User)
来源：http://pme.uphjek.com

PHP:  $u instanceof User
来源：http://hnu.jinghuilouyu.cn

JS:   u instanceof User
来源：http://hxv.jqgfzy.top

TS:   u instanceof User
来源：http://vrg.shuidangran.top

Java: u instanceof User
来源：http://tkn.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eug.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://hhb.dianchejie.cn

C#:   u is User
来源：http://grn.cheryme.top

[G14] 数据类 / record
来源：http://dfl.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vup.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://tks.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://tgh.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://gmd.jianghu66.top

Java: record User(String name, int age) {}
来源：http://ohi.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://vng.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fdt.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://gsv.tarul.cn

[G15] 枚举
来源：http://hgd.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ecm.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sda.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://smi.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yiu.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://crx.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rdz.gogol.net.cn


<!-- 参考信息 -->