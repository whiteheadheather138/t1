代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zak.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vvz.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://aio.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ryo.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://hff.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ayy.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ixg.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqo.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://enx.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wwc.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ijb.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ico.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pzj.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://toq.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ofg.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://drn.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gpa.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vrg.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gch.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ofg.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pln.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mno.svipenyu.cn

[E16] 数字千分位
来源：http://xxr.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://gwf.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://qsa.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rna.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ria.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bzr.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rub.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hzv.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://azq.chenlongwang.top

[E17] 首字母大写
来源：http://vdi.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vpt.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://icy.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://prp.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rlp.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hpq.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ogz.316326.xyz

Ruby: s.capitalize
来源：http://eyx.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tps.ybcxt.top

[E18] 模板占位符替换
来源：http://frz.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jfd.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kwx.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cam.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://eif.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rck.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pko.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ryq.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://txv.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://xxi.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://ekp.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rfm.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://wya.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://jdd.gogol.net.cn

Java: s.lines().toList()
来源：http://krj.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://bcs.sysykeji.top

Ruby: s.lines
来源：http://ubp.xziqi.cn

C#:   s.Split('\n')
来源：http://mvk.tian-w.cn

[E20] 判断字符串是否为空
来源：http://twu.yfazqb.com

Py:   if not s:
来源：http://qup.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wjd.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mju.iojbl.cn

TS:   if (s === "") {}
来源：http://jna.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://shg.cashguo.top

Go:   if s == "" {}
来源：http://jrh.ybcxt.top

Ruby: if s.empty?
来源：http://jtz.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jwx.wangdashe.top

[E21] 超长截断加省略号
来源：http://avd.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ouk.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fdx.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nla.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yto.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://usy.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://vkj.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tdn.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://svg.yonumen.top

[E22] 字节长度与字符长度
来源：http://rea.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ivy.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rom.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aty.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://njt.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cbz.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mxr.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://mha.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ldj.ydzc1.top

================================================================================
来源：http://ovb.ywan-chungtsiang.top

F. 文件与目录
来源：http://uhy.jiagoushi.top

================================================================================
来源：http://bfv.sxryk.cn

[F01] 读取整个文件
来源：http://flb.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jth.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://mzl.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rwr.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nhc.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wug.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xis.jianghu66.top

Ruby: File.read("a.txt")
来源：http://bgi.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://jwq.0kj1m.cn

[F02] 逐行读取文件
来源：http://rlk.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wna.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cbm.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nuf.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tst.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ith.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://djl.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fxx.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bxj.uphjek.com

[F03] 写入文件（覆盖）
来源：http://zwe.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://phx.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://wgh.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://koh.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aii.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bqb.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wzh.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://yjz.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vvo.quarkkingdee.top

[F04] 追加写入文件
来源：http://dwo.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://huk.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sxk.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://akq.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdp.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gyv.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qpp.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qvr.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ypg.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://muv.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bde.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://ymk.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://rfc.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://jtq.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fvf.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bwo.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://oyy.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://vtq.quarkkingdee.top

[F06] 删除文件
来源：http://wfx.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://yas.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://rut.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vlk.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://bvx.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pkc.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://fky.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://rsz.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://oub.xuanzx.com

[F07] 创建目录（含多级）
来源：http://qlw.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ske.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pdh.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rnl.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uyq.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://syq.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ofs.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ure.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xnq.gaohongyu789.top

[F08] 遍历目录
来源：http://gmk.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fga.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vtm.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://ghm.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://vvy.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xdj.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ted.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://hgx.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://iov.cqqwz.cn

[F09] 获取文件大小
来源：http://gmy.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://onj.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://vkm.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://jhr.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://gds.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://hdl.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cdc.fehbvm.com

Ruby: File.size("a.txt")
来源：http://ynl.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://zmb.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://svh.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ruw.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nrm.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xte.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://pyq.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hgg.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zux.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iek.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wll.xuanzx.com

[F11] 复制与移动文件
来源：http://fcj.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cxn.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wen.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aoa.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aqc.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cox.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://who.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iaw.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xgg.xuetiantiany.cn

[F12] CSV 读写
来源：http://uxr.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fqh.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kiv.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uuo.yuxming.cn

TS:   // 同上
来源：http://yxz.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jtm.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bqv.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baa.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://koh.hfpthk.cn

================================================================================
来源：http://sgi.shanyushiyangkeji.top

G. 面向对象
来源：http://gur.vehdjk.com

================================================================================
来源：http://ids.jinqigufen.top

[G01] 定义类
来源：http://swr.ydzc1.top

Py:   class User: pass
来源：http://pxh.jyoumei.cn

PHP:  class User {}
来源：http://kvq.hesvh.cn

JS:   class User {}
来源：http://wfq.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://drs.zhijiandao.cn

Java: class User {}
来源：http://wat.wangdashe.top

Go:   type User struct { Name string }
来源：http://uyh.chenlongwang.top

Ruby: class User; end
来源：http://esm.xinyue.icu

C#:   class User {}
来源：http://xyr.pycfn.com

[G02] 构造函数
来源：http://rsq.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://zss.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://pwp.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://hmm.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://iwx.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://rjs.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vps.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://ozg.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://fsw.hywenlv.cn

[G03] 实例属性
来源：http://nvy.hysaishi.cn

Py:   self.name = "x"
来源：http://cey.havefunace.top

PHP:  public string $name = "x";
来源：http://ihq.hfpthk.cn

JS:   this.name = "x";
来源：http://ume.316326.xyz

TS:   name: string = "x";
来源：http://gpp.jqgfzy.top

Java: private String name;
来源：http://tit.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ghx.yj20258888.top

Ruby: @name = "x"
来源：http://utv.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://fih.yuanzhike.top

[G04] 定义方法
来源：http://yan.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://cet.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rxw.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://mvi.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://yks.daria6918.cn

Java: String greet() { return name; }
来源：http://gxp.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lnd.hnqzz.top

Ruby: def greet; @name; end
来源：http://tck.fzhhl.top

C#:   public string Greet() => Name;
来源：http://vjy.sufxvd.cn

[G05] 继承
来源：http://lws.shuidangran.top

Py:   class Admin(User): pass
来源：http://pqp.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://hna.yj20258888.top

JS:   class Admin extends User {}
来源：http://kom.yuxming.cn

TS:   class Admin extends User {}
来源：http://upb.shanyushiyangkeji.top

Java: class Admin extends User {}
来源：http://sir.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yez.hammf.cn

Ruby: class Admin < User; end
来源：http://rbh.hcnkem.com

C#:   class Admin : User {}
来源：http://xzu.ivvv.top

[G06] 重写方法
来源：http://mfb.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://lis.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zba.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://ewk.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://nnw.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://xfj.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cyp.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://rxv.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://ndc.nanxinkj.top

[G07] 调用父类方法
来源：http://haf.c1oappe.top

Py:   super().greet()
来源：http://bbe.tanke756.top

PHP:  parent::greet();
来源：http://eul.fktsv.cn

JS:   super.greet();
来源：http://hui.yuxming.cn

TS:   super.greet();
来源：http://xgv.sweek.top

Java: super.greet();
来源：http://klx.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kcn.xziqi.cn

Ruby: super
来源：http://xpw.ehwqpu.com

C#:   base.Greet();
来源：http://nqx.yueranfly.top

[G08] 静态方法与属性
来源：http://myd.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xjw.haohaochexian.top

PHP:  public static function f() {}
来源：http://cyi.0kj1m.cn

JS:   static f() {}
来源：http://nrp.zhoulong.xyz

TS:   static f(): void {}
来源：http://fvd.jinghuilouyu.cn

Java: static void f() {}
来源：http://mdx.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yeg.hesvh.cn

Ruby: def self.f; end
来源：http://eqk.jyoumei.cn

C#:   public static void F() {}
来源：http://cnp.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://spw.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://wrn.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vto.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://iay.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://egu.yvedp.cn

Java: interface Shape { double area(); }
来源：http://dyt.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://yob.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwn.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://muo.tanke756.top

[G10] 访问控制
来源：http://cad.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://rwo.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://shc.sysykeji.top

JS:   #private 字段；其余公开
来源：http://hsx.jinqigufen.top

TS:   public / protected / private
来源：http://wua.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://rdj.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nfd.ctjpmb.com

Ruby: public / protected / private
来源：http://ycz.yonumen.top

C#:   public / protected / private / internal
来源：http://bzx.zhongyouzk.top

[G11] getter / setter
来源：http://xgp.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://arl.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rmu.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://fnn.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://azm.0kj1m.cn

Java: public String getName() { return name; }
来源：http://hvl.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://oqf.hfpthk.cn

Ruby: attr_accessor :name
来源：http://zus.guannengcc.top

C#:   public string Name { get; set; }
来源：http://yie.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://kbc.uphjek.com

Py:   def __str__(self): return self.name
来源：http://mkf.vehdjk.com


<!-- 参考信息 -->