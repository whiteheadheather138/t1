代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ikk.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zbr.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kco.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hrz.smart0.xyz

[E14] URL 编码与 Base64
来源：http://rwj.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://adm.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pgp.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://apf.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dni.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qxj.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wpr.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ynf.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://djs.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://ysx.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dzu.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qmy.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eyr.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gpq.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mst.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://udr.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tth.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ejw.guowangkeji.top

[E16] 数字千分位
来源：http://buw.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://xqs.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://gch.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://xow.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jiz.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gbj.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://emp.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cdv.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://vws.nwbrower.top

[E17] 首字母大写
来源：http://ooa.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iqy.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vht.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hdm.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ymm.yj20258888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mbr.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mil.gogol.net.cn

Ruby: s.capitalize
来源：http://gvw.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aph.hcnkem.com

[E18] 模板占位符替换
来源：http://hhu.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ske.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aod.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://psh.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pji.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rvn.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cqt.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://orz.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dbg.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://isv.yonumen.top

Py:   s.splitlines()
来源：http://qtn.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mqk.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://adh.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://tjr.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://jgr.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://szv.zycfv.cn

Ruby: s.lines
来源：http://zoi.vehdjk.com

C#:   s.Split('\n')
来源：http://uik.wangdashe.top

[E20] 判断字符串是否为空
来源：http://atc.chenjidiqi.icu

Py:   if not s:
来源：http://bfk.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jho.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dhg.xinyue.icu

TS:   if (s === "") {}
来源：http://poh.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://qbj.jyoumei.cn

Go:   if s == "" {}
来源：http://dxj.yongpay.top

Ruby: if s.empty?
来源：http://bws.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pvf.vehdjk.com

[E21] 超长截断加省略号
来源：http://adg.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hox.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rhh.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://enc.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzl.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oup.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://wkr.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mlp.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dul.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://ofi.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rfm.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ypw.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fdj.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zee.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://znw.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xph.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://miz.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kdu.daria6918.cn

================================================================================
来源：http://umd.gogol.net.cn

F. 文件与目录
来源：http://vvh.sufxvd.cn

================================================================================
来源：http://rrw.daria6918.cn

[F01] 读取整个文件
来源：http://nph.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ntl.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://wfb.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zhj.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dzu.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fip.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://odv.zycfv.cn

Ruby: File.read("a.txt")
来源：http://hsg.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lzj.jianghu66.top

[F02] 逐行读取文件
来源：http://nyw.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://olh.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ieb.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ntv.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iow.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pmz.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://utk.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rkw.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dxr.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://rzi.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vun.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kme.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kkh.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnf.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nzh.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wkz.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://guq.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dxc.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://lua.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://chw.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dwr.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfc.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yda.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vxt.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oqd.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ghg.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cbv.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://pbz.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://whe.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://ssc.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://xhu.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://ywg.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sjp.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xen.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://dih.sweek.top

C#:   File.Exists("a.txt")
来源：http://ioj.yueranfly.top

[F06] 删除文件
来源：http://ytq.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://mtw.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://mtq.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nyj.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://tri.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://syu.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://ktd.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://xzl.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://kuk.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://kpi.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dyq.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ups.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pum.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mze.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kkt.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://axk.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xpi.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tbj.9152youxi.cn

[F08] 遍历目录
来源：http://xgn.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nev.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zxr.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://ngt.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://kaa.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tae.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://gpm.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://mpw.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://daz.cucudq.cn

[F09] 获取文件大小
来源：http://aqa.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://kfp.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://pzl.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://mpo.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://vpo.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://sux.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yln.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://txo.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://psh.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://xal.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fxj.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://egv.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://obj.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://ojn.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ard.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzh.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://viy.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bsz.fehbvm.com

[F11] 复制与移动文件
来源：http://djs.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cau.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fsq.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gjx.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqb.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kiw.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://end.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ovy.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zrc.tanke756.top

[F12] CSV 读写
来源：http://mrk.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rrl.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://guz.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eow.fanxiaobao.xyz

TS:   // 同上
来源：http://xwv.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://awk.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nui.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yos.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oav.zhaomingkeji.xyz

================================================================================
来源：http://rcq.hnxiangtu.top

G. 面向对象
来源：http://pns.chenjidiqi.icu

================================================================================
来源：http://vtu.chenjidiqi.icu

[G01] 定义类
来源：http://bba.xziqi.cn

Py:   class User: pass
来源：http://hjl.gzhubu.top

PHP:  class User {}
来源：http://zge.ivvv.top

JS:   class User {}
来源：http://fsz.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://sbh.zdqjudy.top

Java: class User {}
来源：http://qcg.sweek.top

Go:   type User struct { Name string }
来源：http://unx.sjlbkw.cn

Ruby: class User; end
来源：http://nji.xylfe.cn

C#:   class User {}
来源：http://ylx.cashguo.top

[G02] 构造函数
来源：http://nnl.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://egk.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://qlf.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://quq.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://ejk.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://wee.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://him.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://gas.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://fms.ivvv.top

[G03] 实例属性
来源：http://goh.kuanghao11.cn

Py:   self.name = "x"
来源：http://jgo.zdqjudy.top

PHP:  public string $name = "x";
来源：http://jjk.dianchejie.cn

JS:   this.name = "x";
来源：http://tlo.snrcjt.cn

TS:   name: string = "x";
来源：http://blm.316326.xyz

Java: private String name;
来源：http://rsx.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://svh.jinqigfzy.top

Ruby: @name = "x"
来源：http://det.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://mzw.wangdashe.top

[G04] 定义方法
来源：http://jlc.c1oappe.top

Py:   def greet(self): return self.name
来源：http://vxd.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yza.yfazqb.com

JS:   greet() { return this.name; }
来源：http://pnr.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://ghq.tanke756.top

Java: String greet() { return name; }
来源：http://jco.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hqn.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://lra.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://aho.fengsongda.top

[G05] 继承
来源：http://uiy.zycfv.cn

Py:   class Admin(User): pass
来源：http://dyh.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://vsl.fktsv.cn

JS:   class Admin extends User {}
来源：http://zqq.birdmap.top

TS:   class Admin extends User {}
来源：http://cpz.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://oyy.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xqa.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://ilf.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://fwh.havefunace.top

[G06] 重写方法
来源：http://pde.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://vav.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://aww.pycfn.com

JS:   greet() { return "admin"; }
来源：http://igg.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://pmf.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://qrc.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nuk.pycfn.com

Ruby: def greet; "admin"; end
来源：http://mwn.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://lqn.redwolf501.top

[G07] 调用父类方法
来源：http://fsa.ppjwa.cn

Py:   super().greet()
来源：http://ugi.yj202588.top

PHP:  parent::greet();
来源：http://gvt.cqqwz.cn

JS:   super.greet();
来源：http://yvk.zhixingplan.top

TS:   super.greet();
来源：http://oma.nanxuanxn.top

Java: super.greet();
来源：http://big.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezu.wangshuangyany.cn

Ruby: super
来源：http://azr.zhixingplan.top

C#:   base.Greet();
来源：http://whc.zhongyouzk.top

[G08] 静态方法与属性
来源：http://sbz.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mut.havefunace.top

PHP:  public static function f() {}
来源：http://asw.xuetiantiany.cn

JS:   static f() {}
来源：http://zwe.yj20258.top

TS:   static f(): void {}
来源：http://bop.ehwqpu.com

Java: static void f() {}
来源：http://fnf.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rkc.ctjpmb.com

Ruby: def self.f; end
来源：http://fco.hywenlv.cn

C#:   public static void F() {}
来源：http://nww.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://ilu.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://rof.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://rcg.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://joa.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://jpj.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://xbn.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://zpk.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ygf.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://mux.hywenlv.cn

[G10] 访问控制
来源：http://fkt.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://otf.aizwys.cn

PHP:  public / protected / private
来源：http://tsy.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://vxs.xuetiantiany.cn

TS:   public / protected / private
来源：http://yvc.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://wlg.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uah.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://cim.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://ibk.sweek.top

[G11] getter / setter
来源：http://ctj.guannengcc.top

Py:   @property 与 @x.setter
来源：http://elx.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qrh.hnqzz.top

JS:   get name() { return this._name; }
来源：http://zrr.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://wxl.ctjpmb.com

Java: public String getName() { return name; }
来源：http://uts.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cja.sufxvd.cn

Ruby: attr_accessor :name
来源：http://qdm.cheryme.top

C#:   public string Name { get; set; }
来源：http://wxz.9152youxi.cn

[G12] 对象转字符串
来源：http://btz.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://xgc.cashguo.top


<!-- 参考信息 -->