代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yqz.sweek.top

[E15] HTML 转义 / 反转义
来源：http://ctm.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://trm.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qhm.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mrf.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vlb.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ati.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cwb.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ody.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fyw.guowangkeji.top

[E16] 数字千分位
来源：http://sgd.mhx1999.top

Py:   f"{1234567:,}"
来源：http://vjf.xylfe.cn

PHP:  number_format(1234567);
来源：http://dtb.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wbd.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://hqu.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tpj.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qwl.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhb.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://evv.sysykeji.top

[E17] 首字母大写
来源：http://gaw.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tcc.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aon.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upk.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qaq.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lxn.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kgb.daxiang520.top

Ruby: s.capitalize
来源：http://kjn.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://igt.svipenyu.cn

[E18] 模板占位符替换
来源：http://kli.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yyp.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rhs.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://svb.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lei.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cbx.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oxw.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bur.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jcb.ydzc1.top

[E19] 多行文本按行拆分
来源：http://wjl.redwolf501.top

Py:   s.splitlines()
来源：http://vid.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uzt.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://cxg.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://wmg.guannengcc.top

Java: s.lines().toList()
来源：http://kpb.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://fru.hesvh.cn

Ruby: s.lines
来源：http://smc.hywenlv.cn

C#:   s.Split('\n')
来源：http://amt.ivvv.top

[E20] 判断字符串是否为空
来源：http://bec.yfazqb.com

Py:   if not s:
来源：http://cwr.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bdh.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bpx.zhixingplan.top

TS:   if (s === "") {}
来源：http://wxp.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://jpx.ppjwa.cn

Go:   if s == "" {}
来源：http://noj.cashguo.top

Ruby: if s.empty?
来源：http://yid.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bbe.tian-w.cn

[E21] 超长截断加省略号
来源：http://stk.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xtg.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kyh.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jcd.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://goi.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oxw.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://hpj.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ylx.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zqi.yvedp.cn

[E22] 字节长度与字符长度
来源：http://iuj.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://epa.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hqn.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://paj.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zlq.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rcw.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kix.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://rrv.zhiwuduotai.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ahk.shzxlz.cn

================================================================================
来源：http://wpf.jinqigufen.top

F. 文件与目录
来源：http://pku.jqgfzy.top

================================================================================
来源：http://eco.bjfxy.top

[F01] 读取整个文件
来源：http://zce.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fjt.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://giq.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fwm.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://odf.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kqr.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wzn.fzhhl.top

Ruby: File.read("a.txt")
来源：http://fnd.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://eel.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://gfd.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bow.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://stf.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tkn.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xap.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yox.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://scc.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sux.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://etf.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://cil.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ymj.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gom.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qmq.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dei.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mrh.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vpo.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://enm.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xuc.ehwqpu.com

[F04] 追加写入文件
来源：http://jis.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://udb.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rnd.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://urr.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zem.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tvv.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gpi.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sge.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://exn.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://xyb.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cfj.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://etw.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://sxz.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://sla.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ptx.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ldl.sweek.top

Ruby: File.exist?("a.txt")
来源：http://yyu.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://wzh.bbcook.cn

[F06] 删除文件
来源：http://qin.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://cgn.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://lal.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://cwx.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://orc.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dig.cashguo.top

Go:   os.Remove("a.txt")
来源：http://dfy.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://ipz.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://aqe.hammf.cn

[F07] 创建目录（含多级）
来源：http://bph.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rwd.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://shv.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjp.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sgs.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jlx.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uwk.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mpj.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ccl.ppjwa.cn

[F08] 遍历目录
来源：http://agl.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dxl.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cww.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://zsm.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://vbm.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eqz.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://snq.aizwys.cn

Ruby: Dir.children("dir")
来源：http://uus.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://iyo.cashguo.top

[F09] 获取文件大小
来源：http://jam.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://vnx.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://uop.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://ffe.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://wuo.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://gnv.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://irc.cheryme.top

Ruby: File.size("a.txt")
来源：http://axr.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://sqv.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://yja.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lky.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ten.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zrp.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://ykv.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://awm.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lxp.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://myb.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bnu.nanxinkj.top

[F11] 复制与移动文件
来源：http://uqn.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cqp.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xtn.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xxf.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szs.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uic.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://trg.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gqz.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uot.ybcxt.top

[F12] CSV 读写
来源：http://ejo.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gdo.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kav.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qty.bbcook.cn

TS:   // 同上
来源：http://beu.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lhw.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dkz.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://szd.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kzi.jqgfzy.top

================================================================================
来源：http://ggb.sxryk.cn

G. 面向对象
来源：http://jix.sjlbkw.cn

================================================================================
来源：http://scm.9152youxi.cn

[G01] 定义类
来源：http://xjl.quarkkingdee.top

Py:   class User: pass
来源：http://ypq.jiagoushi.top

PHP:  class User {}
来源：http://qfe.fzhhl.top

JS:   class User {}
来源：http://miu.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://uhq.zhongyouzk.top

Java: class User {}
来源：http://unk.bbcook.cn

Go:   type User struct { Name string }
来源：http://wqu.xylfe.cn

Ruby: class User; end
来源：http://gxq.jqgfzy.top

C#:   class User {}
来源：http://pyl.hongshengwenyu.top

[G02] 构造函数
来源：http://lhg.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://fqc.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://lpn.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://csw.hammf.cn

TS:   constructor(public name: string) {}
来源：http://zqs.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://ivs.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rwo.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://hzd.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://kxo.316326.xyz

[G03] 实例属性
来源：http://pzm.gotoacloud.top

Py:   self.name = "x"
来源：http://ewf.jyoumei.cn

PHP:  public string $name = "x";
来源：http://mia.ydjk.org.cn

JS:   this.name = "x";
来源：http://nnd.zycfv.cn

TS:   name: string = "x";
来源：http://yak.jlsjyb.cn

Java: private String name;
来源：http://hbm.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rcl.shangyingyoupin.top

Ruby: @name = "x"
来源：http://qjv.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://vjo.sjlbkw.cn

[G04] 定义方法
来源：http://zfn.epnwcf.com

Py:   def greet(self): return self.name
来源：http://olv.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://wtp.yueranfly.top

JS:   greet() { return this.name; }
来源：http://nwl.sweek.top

TS:   greet(): string { return this.name; }
来源：http://bgj.gogol.net.cn

Java: String greet() { return name; }
来源：http://nlu.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://umt.dashuyun.cn

Ruby: def greet; @name; end
来源：http://erw.birdmap.top

C#:   public string Greet() => Name;
来源：http://sun.shzxlz.cn

[G05] 继承
来源：http://lcb.tarul.cn

Py:   class Admin(User): pass
来源：http://ghn.316326.xyz

PHP:  class Admin extends User {}
来源：http://qon.nanxinkj.top

JS:   class Admin extends User {}
来源：http://cuo.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://psd.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://cqa.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lzv.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://wdm.jianghu66.top

C#:   class Admin : User {}
来源：http://sxx.havefunace.top

[G06] 重写方法
来源：http://pau.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://ctx.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://cpx.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://ski.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://wim.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://qmn.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ovy.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://dqf.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://djs.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://hoa.xuanzx.com

Py:   super().greet()
来源：http://gia.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://nns.xziqi.cn

JS:   super.greet();
来源：http://hra.fktsv.cn

TS:   super.greet();
来源：http://rlo.cqqwz.cn

Java: super.greet();
来源：http://ibw.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yht.zhixingplan.top

Ruby: super
来源：http://nfm.dashuyun.cn

C#:   base.Greet();
来源：http://spy.wangdashe.top

[G08] 静态方法与属性
来源：http://yet.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://abx.nanxinkj.top

PHP:  public static function f() {}
来源：http://tmc.jinyuanbaomall.cn

JS:   static f() {}
来源：http://kyg.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://idt.svipenyu.cn

Java: static void f() {}
来源：http://nfy.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://inx.fzhhl.top

Ruby: def self.f; end
来源：http://ncg.xylfe.cn

C#:   public static void F() {}
来源：http://kot.hammf.cn

[G09] 接口 / 抽象类
来源：http://jay.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://ynh.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://rhx.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://oae.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://myu.ydzc1.top

Java: interface Shape { double area(); }
来源：http://udm.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://clc.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xvq.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://xgw.birdmap.top

[G10] 访问控制
来源：http://fct.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://vxu.yj20258888.top

PHP:  public / protected / private
来源：http://iir.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://rxp.hfpthk.cn

TS:   public / protected / private
来源：http://wmg.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://aun.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zhi.andypj.xyz

Ruby: public / protected / private
来源：http://kyq.chenzaomai.com

C#:   public / protected / private / internal
来源：http://kfc.andypj.xyz

[G11] getter / setter
来源：http://eoe.xziqi.cn

Py:   @property 与 @x.setter
来源：http://bzs.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://odf.redwolf501.top

JS:   get name() { return this._name; }
来源：http://vns.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://xrm.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://ael.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ffo.hfpthk.cn

Ruby: attr_accessor :name
来源：http://gfk.c1oappe.top

C#:   public string Name { get; set; }
来源：http://bgy.kuanghao11.cn

[G12] 对象转字符串
来源：http://wln.yonumen.top

Py:   def __str__(self): return self.name
来源：http://tyx.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dne.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://gqw.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://crc.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://car.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://wic.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://fks.yj20258.top

C#:   public override string ToString() => Name;
来源：http://wmq.9152youxi.cn

[G13] 判断对象类型
来源：http://lpm.bjfxy.top

Py:   isinstance(u, User)
来源：http://vmh.yj202588.top

PHP:  $u instanceof User
来源：http://tmh.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://qwk.yj20258.top

TS:   u instanceof User
来源：http://evf.guowangkeji.top


<!-- 参考信息 -->