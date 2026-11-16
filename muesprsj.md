代发 wailian999

PHP:  number_format(1234567);
来源：http://nyx.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rna.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jjb.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eaj.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wwm.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bdx.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://juc.hesvh.cn

[E17] 首字母大写
来源：http://bbi.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hza.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ixd.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqy.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swd.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://idn.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xrg.cucudq.cn

Ruby: s.capitalize
来源：http://ocf.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bza.yvedp.cn

[E18] 模板占位符替换
来源：http://dbm.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iok.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ivy.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tfb.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gvw.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://akc.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aay.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aev.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lay.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://uwh.shzxlz.cn

Py:   s.splitlines()
来源：http://dxx.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://idk.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://zqo.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://tpq.yj20258888.top

Java: s.lines().toList()
来源：http://ejw.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://oyw.gotoacloud.top

Ruby: s.lines
来源：http://iru.sufxvd.cn

C#:   s.Split('\n')
来源：http://mlr.andypj.xyz

[E20] 判断字符串是否为空
来源：http://ssm.zhixingplan.top

Py:   if not s:
来源：http://ost.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bny.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ipc.yangfankeji.com

TS:   if (s === "") {}
来源：http://xmm.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://dck.yuanzhike.top

Go:   if s == "" {}
来源：http://yjk.dashuyun.cn

Ruby: if s.empty?
来源：http://lcw.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pns.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://jnp.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hrc.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bfn.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bcx.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oji.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ojk.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://elr.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uix.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gce.shuidangran.top

[E22] 字节长度与字符长度
来源：http://dye.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cob.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vmp.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://syr.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxh.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ztv.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pje.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://cud.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwe.chenjidiqi.icu

================================================================================
来源：http://ugg.jiagoushi.top

F. 文件与目录
来源：http://qio.shangyingyoupin.top

================================================================================
来源：http://acj.vqdsnc.cn

[F01] 读取整个文件
来源：http://gru.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lhp.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://ybo.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxm.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ryd.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rtc.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dei.fzhhl.top

Ruby: File.read("a.txt")
来源：http://ooz.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://wuu.zhoulong.xyz

[F02] 逐行读取文件
来源：http://kcz.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yyb.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tqp.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ela.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gbp.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qny.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xvw.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukv.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vdm.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://dmp.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tnh.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fai.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mcd.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bht.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bmp.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gmj.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://upo.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nne.zdbjq.cn

[F04] 追加写入文件
来源：http://max.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tmy.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ckg.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://byq.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mri.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iqs.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oii.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cab.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ztv.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://sqf.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xqm.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://stz.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://dhs.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://qbb.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uah.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pfd.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://jrh.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://uic.redwolf501.top

[F06] 删除文件
来源：http://jcs.yongpay.top

Py:   os.remove("a.txt")
来源：http://evv.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://mhz.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://yhy.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://tmh.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bha.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://dnw.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://uxc.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://hbh.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://cvd.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cke.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mqr.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ncd.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sec.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hao.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qci.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pyt.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://abq.xylfe.cn

[F08] 遍历目录
来源：http://hyv.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqk.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wrp.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://nsm.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://mox.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://drf.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nnu.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://ihd.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://eck.zhoulong.xyz

[F09] 获取文件大小
来源：http://vgp.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://kfl.hnqzz.top

PHP:  filesize("a.txt");
来源：http://skv.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://hil.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://nku.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://bmb.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vic.andypj.xyz

Ruby: File.size("a.txt")
来源：http://hmu.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://xzq.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://rmb.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jox.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sjd.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gds.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://ary.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jdq.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vci.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vxn.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qci.birdmap.top

[F11] 复制与移动文件
来源：http://xgr.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bkv.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lbz.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hfc.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ppf.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://drk.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yal.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lkl.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jri.aibaodan.cn

[F12] CSV 读写
来源：http://ukk.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ndr.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wri.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qgx.dianchejie.cn

TS:   // 同上
来源：http://pnd.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cof.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dbe.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cli.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://duf.xinyue.icu

================================================================================
来源：http://pzp.hysaishi.cn

G. 面向对象
来源：http://ckv.9152youxi.cn

================================================================================
来源：http://ycm.gogol.net.cn

[G01] 定义类
来源：http://dno.hfpthk.cn

Py:   class User: pass
来源：http://zlj.316326.xyz

PHP:  class User {}
来源：http://ald.hongshengwenyu.top

JS:   class User {}
来源：http://rci.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://thm.mhx1999.top

Java: class User {}
来源：http://nvj.yj20258.top

Go:   type User struct { Name string }
来源：http://hvw.hywenlv.cn

Ruby: class User; end
来源：http://foo.hnqzz.top

C#:   class User {}
来源：http://onn.wangdashe.top

[G02] 构造函数
来源：http://sie.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://lew.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://qxh.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://tvk.hammf.cn

TS:   constructor(public name: string) {}
来源：http://agt.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://rzp.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wye.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://iko.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://emz.hnqzz.top

[G03] 实例属性
来源：http://ifj.quarkkingdee.top

Py:   self.name = "x"
来源：http://ztl.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://pjh.wangdashe.top

JS:   this.name = "x";
来源：http://cgz.hfpthk.cn

TS:   name: string = "x";
来源：http://dkf.jqgfzy.top

Java: private String name;
来源：http://tyx.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pbi.vehdjk.com

Ruby: @name = "x"
来源：http://fzz.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://iog.sweek.top

[G04] 定义方法
来源：http://bds.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://qdi.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://xfn.shuidangran.top

JS:   greet() { return this.name; }
来源：http://puu.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://dei.xylfe.cn

Java: String greet() { return name; }
来源：http://rty.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://frd.mhx1999.top

Ruby: def greet; @name; end
来源：http://dvz.vehdjk.com

C#:   public string Greet() => Name;
来源：http://wsg.bjfxy.top

[G05] 继承
来源：http://yvo.pycfn.com

Py:   class Admin(User): pass
来源：http://oas.nwbrower.top

PHP:  class Admin extends User {}
来源：http://vyo.snrcjt.cn

JS:   class Admin extends User {}
来源：http://tub.hnqzz.top

TS:   class Admin extends User {}
来源：http://rwa.yueranfly.top

Java: class Admin extends User {}
来源：http://fyr.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ysu.316326.xyz

Ruby: class Admin < User; end
来源：http://twd.yj20258888.top

C#:   class Admin : User {}
来源：http://dls.9152youxi.cn

[G06] 重写方法
来源：http://hub.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://nhy.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://jek.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://quc.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://urx.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://tvk.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://heq.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://btx.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://hbu.chenzaomai.com

[G07] 调用父类方法
来源：http://xbe.tianlin.xyz

Py:   super().greet()
来源：http://kta.xuetiantiany.cn

PHP:  parent::greet();
来源：http://nvj.dashuyun.cn

JS:   super.greet();
来源：http://rno.shuidangran.top

TS:   super.greet();
来源：http://yrp.yj20258888.top

Java: super.greet();
来源：http://hda.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lvj.aibaodan.cn

Ruby: super
来源：http://gwa.gaohongyu789.top

C#:   base.Greet();
来源：http://fyg.redwolf501.top

[G08] 静态方法与属性
来源：http://fck.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jak.quarkkingdee.top

PHP:  public static function f() {}
来源：http://edr.daxiang520.top

JS:   static f() {}
来源：http://tvr.9152youxi.cn

TS:   static f(): void {}
来源：http://ltf.yanxiufei.cn

Java: static void f() {}
来源：http://rwp.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cwu.ppjwa.cn

Ruby: def self.f; end
来源：http://qoh.cqqwz.cn

C#:   public static void F() {}
来源：http://qcu.fehbvm.com

[G09] 接口 / 抽象类
来源：http://nfm.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://mcz.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dqe.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://phs.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://nkf.xinyue.icu

Java: interface Shape { double area(); }
来源：http://lxu.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://iuh.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eaf.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://omo.mhx1999.top

[G10] 访问控制
来源：http://wbv.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://yqc.chenzaomai.com

PHP:  public / protected / private
来源：http://gtx.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://fex.wangshuangyany.cn

TS:   public / protected / private
来源：http://ebs.tarul.cn

Java: public / protected / private / 默认包级
来源：http://mdm.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://stw.zhoulong.xyz

Ruby: public / protected / private
来源：http://ozq.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://iuy.pycfn.com

[G11] getter / setter
来源：http://gwg.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://ekm.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gix.ybcxt.top

JS:   get name() { return this._name; }
来源：http://koq.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://bbg.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://lze.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vrg.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://iam.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://std.xuanzx.com

[G12] 对象转字符串
来源：http://arf.yonumen.top

Py:   def __str__(self): return self.name
来源：http://yhw.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://not.shuidangran.top

JS:   toString() { return this.name; }
来源：http://vhq.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://izx.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://wve.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cgl.hammf.cn

Ruby: def to_s; @name; end
来源：http://xnz.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://wnw.xinyue.icu

[G13] 判断对象类型
来源：http://gel.hnqzz.top

Py:   isinstance(u, User)
来源：http://tzm.haohaochexian.top

PHP:  $u instanceof User
来源：http://tea.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://yih.yonumen.top

TS:   u instanceof User
来源：http://seg.tian-w.cn

Java: u instanceof User
来源：http://zbr.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ckx.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://ifj.daria6918.cn

C#:   u is User
来源：http://gvn.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://dri.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jji.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://fic.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fcv.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://fks.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://pcc.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://vou.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hec.zhixingplan.top


<!-- 参考信息 -->