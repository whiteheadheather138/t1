代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://npb.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihz.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ktr.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mal.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qgb.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dlv.dianchejie.cn

Ruby: s.capitalize
来源：http://jmv.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eqx.xylfe.cn

[E18] 模板占位符替换
来源：http://ztk.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vpz.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uml.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://erm.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qfg.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bfb.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wht.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jki.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zlh.redwolf501.top

[E19] 多行文本按行拆分
来源：http://iaf.fzhhl.top

Py:   s.splitlines()
来源：http://joa.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kfm.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://cjb.zdbjq.cn

TS:   s.split(/\r?\n/)
来源：http://rks.hysaishi.cn

Java: s.lines().toList()
来源：http://lmf.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://jmz.sysykeji.top

Ruby: s.lines
来源：http://lrq.andypj.xyz

C#:   s.Split('\n')
来源：http://dty.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://omq.shzxlz.cn

Py:   if not s:
来源：http://duz.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vfg.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wzc.chenlongwang.top

TS:   if (s === "") {}
来源：http://csn.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://bkg.hnxiangtu.top

Go:   if s == "" {}
来源：http://yud.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://ugk.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cnc.yuxming.cn

[E21] 超长截断加省略号
来源：http://byi.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://skg.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xhn.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cov.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rva.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahk.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://xxi.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qmr.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eud.smart0.xyz

[E22] 字节长度与字符长度
来源：http://ymc.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://inm.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fxm.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://loj.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://olm.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zgt.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rek.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://hhv.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uky.fehbvm.com

================================================================================
来源：http://ehq.zycfv.cn

F. 文件与目录
来源：http://xpt.gotoacloud.top

================================================================================
来源：http://iyz.aizwys.cn

[F01] 读取整个文件
来源：http://ypx.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://syg.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://iyp.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tac.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uhl.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hyl.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ldj.yj20258888.top

Ruby: File.read("a.txt")
来源：http://mtm.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://tlc.jyoumei.cn

[F02] 逐行读取文件
来源：http://cbi.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ppo.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czl.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpr.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xog.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xbq.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlj.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nqm.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fge.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://fdj.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hcm.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qkv.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iec.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijn.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ulv.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://puh.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://pza.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wnv.cdnleiting.top

[F04] 追加写入文件
来源：http://wfg.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://njj.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dhu.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tbs.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jsu.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rrt.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://big.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pia.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://efk.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://obi.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oda.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://qkc.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://eew.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://afl.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dht.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jht.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://qny.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://xop.jqgfzy.top

[F06] 删除文件
来源：http://abi.epnwcf.com

Py:   os.remove("a.txt")
来源：http://jkm.birdmap.top

PHP:  unlink("a.txt");
来源：http://gvj.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://zkl.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://cpp.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bhx.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://azx.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://bhi.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://lkr.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://gsa.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lgz.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dey.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://roy.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqj.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cve.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ajv.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tkm.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bcy.yonumen.top

[F08] 遍历目录
来源：http://mbh.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lyz.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jho.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://knn.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://bck.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cmo.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgp.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://uxu.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://xvu.zhongyouzk.top

[F09] 获取文件大小
来源：http://ljw.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://fbt.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://sky.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://dht.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://gpp.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://mpz.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bip.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://zgs.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://net.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://tyd.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mav.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vas.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ezi.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://djl.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kiw.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fkv.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vmn.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aft.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://njc.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://epi.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://teh.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pex.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyv.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zog.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vvy.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rpd.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gzq.guowangkeji.top

[F12] CSV 读写
来源：http://qdk.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mhd.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yxf.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qzj.hesvh.cn

TS:   // 同上
来源：http://ybn.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lod.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rpz.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yod.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://edq.birdmap.top

================================================================================
来源：http://mnl.zdqjudy.top

G. 面向对象
来源：http://vjm.tianlin.xyz

================================================================================
来源：http://utz.svipenyu.cn

[G01] 定义类
来源：http://yvp.yanxiufei.cn

Py:   class User: pass
来源：http://slc.xylfe.cn

PHP:  class User {}
来源：http://rcu.aibaodan.cn

JS:   class User {}
来源：http://jch.uphjek.com

TS:   class User { name: string = ""; }
来源：http://ihl.yj20258.top

Java: class User {}
来源：http://lyi.daxiang520.top

Go:   type User struct { Name string }
来源：http://sxy.fehbvm.com

Ruby: class User; end
来源：http://dde.aibaodan.cn

C#:   class User {}
来源：http://iwh.jinyuanbaomall.cn

[G02] 构造函数
来源：http://gmy.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://fid.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://umd.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://dpn.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://rms.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://haq.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wyc.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://wdg.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://xri.fzhhl.top

[G03] 实例属性
来源：http://dxi.9152youxi.cn

Py:   self.name = "x"
来源：http://mhs.ivvv.top

PHP:  public string $name = "x";
来源：http://zgw.gzhubu.top

JS:   this.name = "x";
来源：http://dfh.daria6918.cn

TS:   name: string = "x";
来源：http://zwh.epnwcf.com

Java: private String name;
来源：http://ctk.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sla.hammf.cn

Ruby: @name = "x"
来源：http://qlf.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://rlq.svipenyu.cn

[G04] 定义方法
来源：http://uqf.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://crl.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xkd.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://tjj.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://hlr.gotoacloud.top

Java: String greet() { return name; }
来源：http://oqi.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mpr.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://rwq.cucudq.cn

C#:   public string Greet() => Name;
来源：http://sli.chenlongwang.top

[G05] 继承
来源：http://ian.fktsv.cn

Py:   class Admin(User): pass
来源：http://cgg.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://rxv.haohaochexian.top

JS:   class Admin extends User {}
来源：http://zof.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://mjo.tanke756.top

Java: class Admin extends User {}
来源：http://xuo.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://osq.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://afz.pycfn.com

C#:   class Admin : User {}
来源：http://jgh.yj202588.top

[G06] 重写方法
来源：http://boi.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://wdn.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://zvf.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://ikb.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://dux.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://pyk.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vzr.yonumen.top

Ruby: def greet; "admin"; end
来源：http://evk.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://jin.xinyue.icu

[G07] 调用父类方法
来源：http://gza.hongshengwenyu.top

Py:   super().greet()
来源：http://pcq.jqgfzy.top

PHP:  parent::greet();
来源：http://mju.jlsjyb.cn

JS:   super.greet();
来源：http://rwa.xuetiantiany.cn

TS:   super.greet();
来源：http://gys.ybcxt.top

Java: super.greet();
来源：http://uob.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ndd.birdmap.top

Ruby: super
来源：http://bpd.gogol.net.cn

C#:   base.Greet();
来源：http://gbu.xziqi.cn

[G08] 静态方法与属性
来源：http://mev.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zuo.kuanghao11.cn

PHP:  public static function f() {}
来源：http://tgl.xuetiantiany.cn

JS:   static f() {}
来源：http://qbg.svipenyu.cn

TS:   static f(): void {}
来源：http://vwl.52xcode.cn

Java: static void f() {}
来源：http://wld.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kxz.daxiang520.top

Ruby: def self.f; end
来源：http://xmz.pycfn.com

C#:   public static void F() {}
来源：http://ybq.bjfxy.top

[G09] 接口 / 抽象类
来源：http://rca.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://jfg.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zwo.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://anp.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://dyy.tarul.cn

Java: interface Shape { double area(); }
来源：http://oan.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://pbc.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://evd.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://bde.jyoumei.cn

[G10] 访问控制
来源：http://kxs.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://usr.hnqzz.top

PHP:  public / protected / private
来源：http://mms.mhx1999.top

JS:   #private 字段；其余公开
来源：http://stq.pengpengdd.cyou

TS:   public / protected / private
来源：http://ekf.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://jrb.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qgo.sjlbkw.cn

Ruby: public / protected / private
来源：http://fls.cucudq.cn

C#:   public / protected / private / internal
来源：http://mob.zhixingplan.top

[G11] getter / setter
来源：http://nyl.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://ebi.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vmd.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://plu.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://fkz.ppjwa.cn

Java: public String getName() { return name; }
来源：http://itw.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sgx.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://wqy.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://zni.snrcjt.cn

[G12] 对象转字符串
来源：http://whs.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://lvo.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://out.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://rdd.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://vgw.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://fyu.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ams.yj20258888.top

Ruby: def to_s; @name; end
来源：http://unq.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://cjw.ydjk.org.cn

[G13] 判断对象类型
来源：http://poo.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://ypu.tanke756.top

PHP:  $u instanceof User
来源：http://gat.aibaodan.cn

JS:   u instanceof User
来源：http://xdo.sysykeji.top

TS:   u instanceof User
来源：http://fna.xziqi.cn

Java: u instanceof User
来源：http://syk.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hsh.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://abm.dashuyun.cn

C#:   u is User
来源：http://qmn.ctjpmb.com

[G14] 数据类 / record
来源：http://jhf.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aru.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://eic.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://res.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://kzb.hnqzz.top

Java: record User(String name, int age) {}
来源：http://udf.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://rgl.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ncl.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://you.sufxvd.cn

[G15] 枚举
来源：http://dns.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pnn.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jui.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lqe.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jry.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://mal.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oky.havefunace.top


<!-- 参考信息 -->