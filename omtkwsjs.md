代发 wailian999

JS:   [...s].reverse().join("")
来源：http://vfk.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://cny.zhoulong.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://hvw.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gha.jianghu66.top

Ruby: s.reverse
来源：http://ekx.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://xtx.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://qqx.yangfankeji.com

Py:   s.count("a")
来源：http://szp.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://jat.cashguo.top

JS:   s.split("a").length - 1
来源：http://eau.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://dyu.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vlg.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://ypy.chenlongwang.top

Ruby: s.count("a")
来源：http://nyj.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://rkh.zhengqikj.top

[E13] 逐字符遍历
来源：http://hwk.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://vag.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tsh.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fhl.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://faj.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gmj.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://krx.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tzb.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://isz.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://zba.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wek.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://voh.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swa.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pad.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qzp.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dhl.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aqq.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ysf.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://ark.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dgu.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rab.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sci.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ucv.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xgm.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ecf.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://spq.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gjl.hesvh.cn

[E16] 数字千分位
来源：http://ojp.xziqi.cn

Py:   f"{1234567:,}"
来源：http://xnq.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://yho.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mhd.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://rtn.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxc.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ght.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnh.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://vxn.xuanzx.com

[E17] 首字母大写
来源：http://oto.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hbq.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oec.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykk.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpu.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ros.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fba.xziqi.cn

Ruby: s.capitalize
来源：http://aum.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dtc.cdnleiting.top

[E18] 模板占位符替换
来源：http://kob.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zqp.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yja.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bmj.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ref.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ylb.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rck.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tkg.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rpg.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://ygx.chenzaomai.com

Py:   s.splitlines()
来源：http://xtv.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ndr.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://msy.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://ssk.yanxiufei.cn

Java: s.lines().toList()
来源：http://ycr.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://vkr.haohaochexian.top

Ruby: s.lines
来源：http://fnr.meibo888.top

C#:   s.Split('\n')
来源：http://iyj.nwbrower.top

[E20] 判断字符串是否为空
来源：http://mfi.sysykeji.top

Py:   if not s:
来源：http://hgt.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zol.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rkq.vqdsnc.cn

TS:   if (s === "") {}
来源：http://jef.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://gch.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://oem.snrcjt.cn

Ruby: if s.empty?
来源：http://ziw.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hnk.haohaochexian.top

[E21] 超长截断加省略号
来源：http://abg.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bcb.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zos.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zpl.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kjp.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hzq.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://div.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mmt.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://obj.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://jcu.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iyu.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vyo.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kfp.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmd.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lca.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ksu.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://xil.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mjw.yonumen.top

================================================================================
来源：http://dth.feifeiyinyue.top

F. 文件与目录
来源：http://afh.dianchejie.cn

================================================================================
来源：http://hoy.9152youxi.cn

[F01] 读取整个文件
来源：http://red.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://phe.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://qav.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vud.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gkb.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://org.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jdd.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://zjh.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://ueg.snrcjt.cn

[F02] 逐行读取文件
来源：http://zwd.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mwx.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ojm.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mxh.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wby.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hyx.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://twb.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vwg.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ujd.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://ltm.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://keh.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://thb.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pkb.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zpe.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mdh.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pjf.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://iqj.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yko.yj20258888.top

[F04] 追加写入文件
来源：http://ckc.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://glg.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sxm.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lah.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://red.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pto.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lnt.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://efr.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ebf.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://bcq.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ooz.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://zyl.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://eyq.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://atk.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ktb.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fgs.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://txg.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://nya.sxryk.cn

[F06] 删除文件
来源：http://geq.52xcode.cn

Py:   os.remove("a.txt")
来源：http://tsj.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://qxn.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://ptw.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://wjx.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fsz.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://rto.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://fcg.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://opb.nwbrower.top

[F07] 创建目录（含多级）
来源：http://beh.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mku.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uxy.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bta.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhk.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://otu.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fyl.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bua.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vxl.yangfankeji.com

[F08] 遍历目录
来源：http://rpd.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://yyp.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://erc.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://dwv.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://yjh.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vqj.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://bru.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://gvf.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://kxp.316326.xyz

[F09] 获取文件大小
来源：http://niv.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://zif.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://aso.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://wbq.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://gdl.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://kqa.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://imn.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://nex.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://chn.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://ugu.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ezd.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://olf.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jgr.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://apj.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rhm.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lwi.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vow.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://utz.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://cei.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ygf.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ckn.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mog.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ukp.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ylb.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rtq.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pnk.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://skh.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://epy.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vpz.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ffb.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vmd.jinqigufen.top

TS:   // 同上
来源：http://uis.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykq.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kvy.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rnt.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tux.zhiwuduotai.top

================================================================================
来源：http://ohn.tian-w.cn

G. 面向对象
来源：http://qsx.iojbl.cn

================================================================================
来源：http://dgk.jiagoushi.top

[G01] 定义类
来源：http://mhi.cucudq.cn

Py:   class User: pass
来源：http://rlj.chenlongwang.top

PHP:  class User {}
来源：http://ikx.yangfankeji.com

JS:   class User {}
来源：http://jci.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://gwh.yj20258888.top

Java: class User {}
来源：http://dbm.cdnleiting.top

Go:   type User struct { Name string }
来源：http://jnt.nwbrower.top

Ruby: class User; end
来源：http://vgv.yuanzhike.top

C#:   class User {}
来源：http://smf.pengpengdd.cyou

[G02] 构造函数
来源：http://brp.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://bjv.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://kpl.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://vps.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://fum.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://dea.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ged.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://gkl.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://pux.haohaochexian.top

[G03] 实例属性
来源：http://bar.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://oal.sysykeji.top

PHP:  public string $name = "x";
来源：http://dok.nanxuanxn.top

JS:   this.name = "x";
来源：http://tuj.smart0.xyz

TS:   name: string = "x";
来源：http://tbs.yuxming.cn

Java: private String name;
来源：http://fru.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yjf.pycfn.com

Ruby: @name = "x"
来源：http://tyq.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://sac.zdqjudy.top

[G04] 定义方法
来源：http://ruk.uphjek.com

Py:   def greet(self): return self.name
来源：http://qat.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yhl.andypj.xyz

JS:   greet() { return this.name; }
来源：http://tah.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://tje.havefunace.top

Java: String greet() { return name; }
来源：http://fos.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://brc.cdnleiting.top

Ruby: def greet; @name; end
来源：http://tik.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://igy.hnxiangtu.top

[G05] 继承
来源：http://jcf.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://phw.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://xii.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://hen.sweek.top

TS:   class Admin extends User {}
来源：http://vka.yfazqb.com

Java: class Admin extends User {}
来源：http://mel.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://koa.havefunace.top

Ruby: class Admin < User; end
来源：http://cgl.nanxuanxn.top

C#:   class Admin : User {}
来源：http://wgm.daxiang520.top

[G06] 重写方法
来源：http://mgv.pycfn.com

Py:   def greet(self): return "admin"
来源：http://jhx.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://uil.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://hco.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://lpx.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://lng.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fut.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://uat.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://ttz.zhijiandao.cn

[G07] 调用父类方法
来源：http://xiq.cashguo.top

Py:   super().greet()
来源：http://omw.fktsv.cn

PHP:  parent::greet();
来源：http://bxs.bbcook.cn

JS:   super.greet();
来源：http://gar.redwolf501.top

TS:   super.greet();
来源：http://uqv.hfpthk.cn

Java: super.greet();
来源：http://yoe.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aem.sweek.top

Ruby: super
来源：http://mxv.jinqigufen.top

C#:   base.Greet();
来源：http://fps.yonumen.top

[G08] 静态方法与属性
来源：http://ipu.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sqy.shzxlz.cn

PHP:  public static function f() {}
来源：http://qea.yj20258.top

JS:   static f() {}
来源：http://kpy.zhoulong.xyz

TS:   static f(): void {}
来源：http://iwl.hnqzz.top

Java: static void f() {}
来源：http://bfw.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fnc.sweek.top

Ruby: def self.f; end
来源：http://trw.nwbrower.top

C#:   public static void F() {}
来源：http://kvb.yongpay.top

[G09] 接口 / 抽象类
来源：http://ueo.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://xvg.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://prg.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vqc.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://jfo.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://vyj.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://dbs.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyi.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://gmd.jinqigfzy.top


<!-- 参考信息 -->