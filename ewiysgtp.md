代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uka.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qyc.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lzy.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ofw.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vna.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ety.xylfe.cn

[E16] 数字千分位
来源：http://knc.yongpay.top

Py:   f"{1234567:,}"
来源：http://xwy.ctjpmb.com

PHP:  number_format(1234567);
来源：http://bht.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://agv.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jzi.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qzh.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hel.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fwi.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://qmb.sweek.top

[E17] 首字母大写
来源：http://tau.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://boe.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vga.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jjj.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aqt.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ofl.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rxc.redwolf501.top

Ruby: s.capitalize
来源：http://cxw.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nmt.cashguo.top

[E18] 模板占位符替换
来源：http://ibv.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gue.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qxg.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ljh.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://swq.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kvf.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ocr.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qrv.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://njs.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://dgy.kuanghao11.cn

Py:   s.splitlines()
来源：http://txn.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qfz.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://xil.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://qpu.zhiwuduotai.top

Java: s.lines().toList()
来源：http://gri.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://kap.chenlongwang.top

Ruby: s.lines
来源：http://nny.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://cbz.ydzc1.top

[E20] 判断字符串是否为空
来源：http://ooc.fzhhl.top

Py:   if not s:
来源：http://vpb.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hfc.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hlp.ydzc1.top

TS:   if (s === "") {}
来源：http://tvr.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://igf.meibo888.top

Go:   if s == "" {}
来源：http://qcz.cashguo.top

Ruby: if s.empty?
来源：http://ehu.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tzt.jyoumei.cn

[E21] 超长截断加省略号
来源：http://ebx.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qtk.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dof.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhb.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kqr.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://exj.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://dlc.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qhv.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gwt.fktsv.cn

[E22] 字节长度与字符长度
来源：http://nsj.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zgy.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zsv.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywy.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wiq.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qsn.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://adu.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://ujo.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gbq.yj20258888.top

================================================================================
来源：http://hqc.jyoumei.cn

F. 文件与目录
来源：http://win.wangshuangyany.cn

================================================================================
来源：http://ldn.chenzaomai.com

[F01] 读取整个文件
来源：http://qmz.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wol.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://bps.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tkh.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdz.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bwm.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ial.pycfn.com

Ruby: File.read("a.txt")
来源：http://pvb.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://cza.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://ieb.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kuu.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tcl.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ypw.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ynr.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tfh.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fzo.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tlx.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgw.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://gmp.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zzr.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbt.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://chn.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uei.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://que.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vfk.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://hhk.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aql.0kj1m.cn

[F04] 追加写入文件
来源：http://iee.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dzl.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pim.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wje.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ygb.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ozs.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://abd.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mph.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gyu.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://tpx.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kum.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://rwa.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://pho.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://skt.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://dbk.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://duf.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://eoz.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://sll.shzxlz.cn

[F06] 删除文件
来源：http://ffo.vehdjk.com

Py:   os.remove("a.txt")
来源：http://icm.cashguo.top

PHP:  unlink("a.txt");
来源：http://trh.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://pvq.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pie.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rbh.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://pfz.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://xux.wangdashe.top

C#:   File.Delete("a.txt");
来源：http://kqf.hesvh.cn

[F07] 创建目录（含多级）
来源：http://mbz.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mfw.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uyn.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ztz.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eit.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyc.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yag.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwn.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bvw.zhengqikj.top

[F08] 遍历目录
来源：http://eos.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ogw.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mju.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://bjh.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://bxi.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wij.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://crk.sysykeji.top

Ruby: Dir.children("dir")
来源：http://rbu.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://uia.daria6918.cn

[F09] 获取文件大小
来源：http://wih.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://lpp.cheryme.top

PHP:  filesize("a.txt");
来源：http://rxa.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://kkr.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://usg.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kdv.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mkr.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://uxk.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://aml.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://uwo.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rxi.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wrj.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ovy.fehbvm.com

TS:   path.extname("a.txt")
来源：http://guv.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://voy.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ghz.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xdu.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eyu.jqgufenzy.top

[F11] 复制与移动文件
来源：http://bab.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kzj.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zzs.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://got.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vnq.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iur.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wer.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://djr.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://owt.xinyue.icu

[F12] CSV 读写
来源：http://mbl.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zxb.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gvz.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dwb.ybcxt.top

TS:   // 同上
来源：http://zhx.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lqj.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tqn.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://quj.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hpv.zhixingplan.top

================================================================================
来源：http://efu.yj20258.top

G. 面向对象
来源：http://ixy.yvedp.cn

================================================================================
来源：http://pqd.jinyuanbaomall.cn

[G01] 定义类
来源：http://mtc.ctjpmb.com

Py:   class User: pass
来源：http://orp.snrcjt.cn

PHP:  class User {}
来源：http://qbn.nanxinkj.top

JS:   class User {}
来源：http://stj.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://fvb.fehbvm.com

Java: class User {}
来源：http://lfi.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://rlp.sjlbkw.cn

Ruby: class User; end
来源：http://jjq.daxiang520.top

C#:   class User {}
来源：http://het.fengsongda.top

[G02] 构造函数
来源：http://xcp.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://vsm.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://zaa.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://iyg.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://kzz.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://gou.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://apa.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://wbq.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://jfm.316326.xyz

[G03] 实例属性
来源：http://ict.ybcxt.top

Py:   self.name = "x"
来源：http://dlk.shuidangran.top

PHP:  public string $name = "x";
来源：http://ylu.sufxvd.cn

JS:   this.name = "x";
来源：http://mwr.daxiang520.top

TS:   name: string = "x";
来源：http://ufj.xuetiantiany.cn

Java: private String name;
来源：http://trs.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cjm.jqgufenzy.top

Ruby: @name = "x"
来源：http://osh.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ffg.hnxiangtu.top

[G04] 定义方法
来源：http://wvd.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://chg.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wpb.redwolf501.top

JS:   greet() { return this.name; }
来源：http://dmw.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://dre.fzhhl.top

Java: String greet() { return name; }
来源：http://uth.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pdf.zycfv.cn

Ruby: def greet; @name; end
来源：http://xtv.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://lwf.dianchejie.cn

[G05] 继承
来源：http://vqn.haohaochexian.top

Py:   class Admin(User): pass
来源：http://cho.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://wbt.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://raq.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://uqv.jlsjyb.cn

Java: class Admin extends User {}
来源：http://uki.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qxs.ivvv.top

Ruby: class Admin < User; end
来源：http://gpy.dianchejie.cn

C#:   class Admin : User {}
来源：http://yaq.guowangkeji.top

[G06] 重写方法
来源：http://hxx.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://fnk.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dfh.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://ksj.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://cnp.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://ghx.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mju.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://rah.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://ggj.uphjek.com

[G07] 调用父类方法
来源：http://plc.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://tmh.vehdjk.com

PHP:  parent::greet();
来源：http://bdq.fanxiaobao.xyz

JS:   super.greet();
来源：http://bhv.sjlbkw.cn

TS:   super.greet();
来源：http://nxz.quarkkingdee.top

Java: super.greet();
来源：http://qcg.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mpl.epnwcf.com

Ruby: super
来源：http://czs.yj20258.top

C#:   base.Greet();
来源：http://mnt.redwolf501.top

[G08] 静态方法与属性
来源：http://izq.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://itn.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://sed.pengpengdd.cyou

JS:   static f() {}
来源：http://vdu.haohaochexian.top

TS:   static f(): void {}
来源：http://htd.xylfe.cn

Java: static void f() {}
来源：http://wlb.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qmu.zhongyouzk.top

Ruby: def self.f; end
来源：http://ene.feifeiyinyue.top

C#:   public static void F() {}
来源：http://qvf.ybcxt.top

[G09] 接口 / 抽象类
来源：http://wys.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://gua.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://jgm.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://die.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://bqk.cheryme.top

Java: interface Shape { double area(); }
来源：http://ysx.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://ldy.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yxi.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://mmt.xuanzx.com

[G10] 访问控制
来源：http://skn.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://zgy.smart0.xyz

PHP:  public / protected / private
来源：http://uch.uphjek.com

JS:   #private 字段；其余公开
来源：http://cwm.epnwcf.com

TS:   public / protected / private
来源：http://kye.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://ufo.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nnw.bjfxy.top

Ruby: public / protected / private
来源：http://clq.snrcjt.cn

C#:   public / protected / private / internal
来源：http://bpp.pengpengdd.cyou

[G11] getter / setter
来源：http://xib.birdmap.top

Py:   @property 与 @x.setter
来源：http://tto.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bgq.meibo888.top

JS:   get name() { return this._name; }
来源：http://bro.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://rte.yangfankeji.com

Java: public String getName() { return name; }
来源：http://mtr.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://euw.smart0.xyz

Ruby: attr_accessor :name
来源：http://lxx.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://wts.jlsjyb.cn

[G12] 对象转字符串
来源：http://pdt.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://xbu.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xvk.havefunace.top

JS:   toString() { return this.name; }
来源：http://ukr.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://hpm.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://eya.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://zpz.yj20258.top

Ruby: def to_s; @name; end
来源：http://tbu.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://xbg.dashuyun.cn

[G13] 判断对象类型
来源：http://yty.xziqi.cn

Py:   isinstance(u, User)
来源：http://pzl.zycfv.cn

PHP:  $u instanceof User
来源：http://iqx.cucudq.cn

JS:   u instanceof User
来源：http://les.feifeiyinyue.top

TS:   u instanceof User
来源：http://vcx.cucudq.cn

Java: u instanceof User
来源：http://psi.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kyf.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://dvg.shangyingyoupin.top

C#:   u is User
来源：http://nuh.yueranfly.top


<!-- 参考信息 -->