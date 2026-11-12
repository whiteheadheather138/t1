代发 wailian999

[E14] URL 编码与 Base64
来源：http://nyr.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mtj.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://yel.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lua.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jxc.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cjo.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tlt.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://htz.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qmt.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://frm.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ytx.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hqu.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mef.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://krt.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hso.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nci.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fwq.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://plo.yuxming.cn

[E16] 数字千分位
来源：http://exm.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://ach.yj20258888.top

PHP:  number_format(1234567);
来源：http://kkw.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qmj.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bzd.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xxf.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pyo.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vec.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://otw.hnxiangtu.top

[E17] 首字母大写
来源：http://bpy.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tji.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://njy.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iky.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kck.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pjj.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fcw.zhiwuduotai.top

Ruby: s.capitalize
来源：http://nmh.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://twz.yongpay.top

[E18] 模板占位符替换
来源：http://ijs.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ats.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xhc.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dkq.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mvn.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bvk.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jme.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cxq.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uhu.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://hnw.sxryk.cn

Py:   s.splitlines()
来源：http://fqr.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vpu.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://gqd.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://eai.guannengcc.top

Java: s.lines().toList()
来源：http://roz.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://tnr.shangyingyoupin.top

Ruby: s.lines
来源：http://lto.yj20258888.top

C#:   s.Split('\n')
来源：http://qxg.sxryk.cn

[E20] 判断字符串是否为空
来源：http://kwj.zdbjq.cn

Py:   if not s:
来源：http://hrj.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://swg.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yzz.aizwys.cn

TS:   if (s === "") {}
来源：http://jhb.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://mse.gogol.net.cn

Go:   if s == "" {}
来源：http://ajk.fengsongda.top

Ruby: if s.empty?
来源：http://ttb.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jth.yueranfly.top

[E21] 超长截断加省略号
来源：http://qwj.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nzg.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://znw.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://don.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kpn.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yld.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://zgc.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://llk.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pxr.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://zil.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hsp.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ltn.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yxe.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnh.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uhn.yj20258888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fnh.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://oad.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uuz.zhengqikj.top

================================================================================
来源：http://mxn.yvedp.cn

F. 文件与目录
来源：http://tga.jlsjyb.cn

================================================================================
来源：http://nmt.zdbjq.cn

[F01] 读取整个文件
来源：http://jjh.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hqk.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://lkz.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ywd.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ucm.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lge.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ucu.bjfxy.top

Ruby: File.read("a.txt")
来源：http://lle.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://wqt.yfazqb.com

[F02] 逐行读取文件
来源：http://qnh.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lib.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrw.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eph.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bhe.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hht.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qop.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ong.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nzk.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://ohq.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jqf.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tvm.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smz.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wos.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bft.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vin.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://qdw.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wby.tian-w.cn

[F04] 追加写入文件
来源：http://pdo.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jrl.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ofv.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pyg.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rxo.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ayg.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fxv.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gvz.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kxp.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://ufn.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cfu.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://emz.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://szg.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://tae.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hrs.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nsq.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://fzt.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://ppl.yonumen.top

[F06] 删除文件
来源：http://zyk.nwbrower.top

Py:   os.remove("a.txt")
来源：http://ryv.fehbvm.com

PHP:  unlink("a.txt");
来源：http://kjh.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uhv.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://huy.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oap.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://rbd.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://uph.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://uux.fktsv.cn

[F07] 创建目录（含多级）
来源：http://vbs.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jir.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://byg.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gmh.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wdn.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uug.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ass.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qgx.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tns.zdbjq.cn

[F08] 遍历目录
来源：http://fvz.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hwg.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ull.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://svp.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://kwl.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wqq.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nma.yueranfly.top

Ruby: Dir.children("dir")
来源：http://ozn.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://hbi.gogol.net.cn

[F09] 获取文件大小
来源：http://sam.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://ume.birdmap.top

PHP:  filesize("a.txt");
来源：http://yhf.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://upi.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://xhm.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bls.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dgi.jianghu66.top

Ruby: File.size("a.txt")
来源：http://unl.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://hsv.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://yir.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://inh.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zps.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ibx.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://fdf.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nsp.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pli.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nmd.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oun.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://znh.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qea.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nxo.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://loh.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pye.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kyu.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ofo.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gis.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qdg.jinghuilouyu.cn

[F12] CSV 读写
来源：http://myl.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gui.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zwn.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ipy.cqqwz.cn

TS:   // 同上
来源：http://czm.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bks.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://psj.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lfm.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zih.meibo888.top

================================================================================
来源：http://ebg.jiagoushi.top

G. 面向对象
来源：http://ufk.xziqi.cn

================================================================================
来源：http://mkg.ehwqpu.com

[G01] 定义类
来源：http://gma.yj20258888.top

Py:   class User: pass
来源：http://mes.hnxiangtu.top

PHP:  class User {}
来源：http://wio.hfpthk.cn

JS:   class User {}
来源：http://wnk.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://nqy.tianlin.xyz

Java: class User {}
来源：http://mmc.sweek.top

Go:   type User struct { Name string }
来源：http://bxs.hywenlv.cn

Ruby: class User; end
来源：http://hjb.iojbl.cn

C#:   class User {}
来源：http://cvn.jianghu66.top

[G02] 构造函数
来源：http://mfg.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://ymc.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://yti.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ixz.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://rdu.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://urt.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vow.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://pez.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://xsu.zdbjq.cn

[G03] 实例属性
来源：http://xfj.cqqwz.cn

Py:   self.name = "x"
来源：http://eqa.guowangkeji.top

PHP:  public string $name = "x";
来源：http://pek.sjlbkw.cn

JS:   this.name = "x";
来源：http://ksz.gotoacloud.top

TS:   name: string = "x";
来源：http://umm.zhongyouzk.top

Java: private String name;
来源：http://doz.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nab.ydjk.org.cn

Ruby: @name = "x"
来源：http://zcz.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://mbm.zhijiandao.cn

[G04] 定义方法
来源：http://jsa.xinyue.icu

Py:   def greet(self): return self.name
来源：http://wta.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ehb.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://hmk.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://vxp.jianghu66.top

Java: String greet() { return name; }
来源：http://jne.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://knz.tarul.cn

Ruby: def greet; @name; end
来源：http://djc.cashguo.top

C#:   public string Greet() => Name;
来源：http://dqn.hnxiangtu.top

[G05] 继承
来源：http://axh.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://iqe.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://wvb.yj20258.top

JS:   class Admin extends User {}
来源：http://hjs.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://orz.fktsv.cn

Java: class Admin extends User {}
来源：http://eju.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bac.bbcook.cn

Ruby: class Admin < User; end
来源：http://qbo.vehdjk.com

C#:   class Admin : User {}
来源：http://knu.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://faw.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://iou.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nmy.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://qhu.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://mek.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://ycj.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eog.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://hcu.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://yau.haohaochexian.top

[G07] 调用父类方法
来源：http://gwo.ydzc1.top

Py:   super().greet()
来源：http://qhf.kuanghao11.cn

PHP:  parent::greet();
来源：http://obf.jinqigufen.top

JS:   super.greet();
来源：http://zjw.jqgfzy.top

TS:   super.greet();
来源：http://tsh.hcnkem.com

Java: super.greet();
来源：http://pxq.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rtu.cucudq.cn

Ruby: super
来源：http://mhm.yj20258888.top

C#:   base.Greet();
来源：http://kcd.316326.xyz

[G08] 静态方法与属性
来源：http://sdn.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pnk.havefunace.top

PHP:  public static function f() {}
来源：http://ohj.fktsv.cn

JS:   static f() {}
来源：http://bvz.jqgfzy.top

TS:   static f(): void {}
来源：http://frv.bbcook.cn

Java: static void f() {}
来源：http://cuc.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://etj.uphjek.com

Ruby: def self.f; end
来源：http://nwb.vehdjk.com

C#:   public static void F() {}
来源：http://mum.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://gwf.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://qqr.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://jum.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wwd.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://dfv.hnqzz.top

Java: interface Shape { double area(); }
来源：http://kui.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://enn.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ccz.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://sau.gogol.net.cn

[G10] 访问控制
来源：http://qiy.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://fgr.chenlongwang.top

PHP:  public / protected / private
来源：http://fzk.sysykeji.top

JS:   #private 字段；其余公开
来源：http://enu.bbcook.cn

TS:   public / protected / private
来源：http://fay.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://rnf.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ffg.zhijiandao.cn

Ruby: public / protected / private
来源：http://san.hywenlv.cn

C#:   public / protected / private / internal
来源：http://gdo.sxryk.cn

[G11] getter / setter
来源：http://vvr.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://spy.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qvm.cashguo.top

JS:   get name() { return this._name; }
来源：http://lva.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://kkv.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://nec.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://old.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://sug.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://oxb.shzxlz.cn

[G12] 对象转字符串
来源：http://pxd.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://htx.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://axv.aizwys.cn

JS:   toString() { return this.name; }
来源：http://nid.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://sog.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://sns.fktsv.cn


<!-- 参考信息 -->