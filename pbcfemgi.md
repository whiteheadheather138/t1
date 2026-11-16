代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://isq.zhoulong.xyz

[E11] 反转字符串
来源：http://ntp.wangshuangyany.cn

Py:   s[::-1]
来源：http://rcf.ppjwa.cn

PHP:  strrev($s);
来源：http://lpj.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://hzi.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://kts.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kug.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qos.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://sun.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sbz.sysykeji.top

[E12] 统计某字符出现次数
来源：http://ksr.meibo888.top

Py:   s.count("a")
来源：http://ghg.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://dbm.c1oappe.top

JS:   s.split("a").length - 1
来源：http://qsp.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://icg.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dmc.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://bbr.epnwcf.com

Ruby: s.count("a")
来源：http://ifa.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://fcu.jianghu66.top

[E13] 逐字符遍历
来源：http://xot.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://uao.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uzz.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://keh.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qps.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sue.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ygx.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mvr.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rxa.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://hpj.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://azn.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://sye.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ago.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://evj.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vsa.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fal.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ong.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jda.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://loq.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://yrt.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://moq.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://opy.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vhm.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyw.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pkb.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lsq.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ftt.bjfxy.top

[E16] 数字千分位
来源：http://pbq.yuxming.cn

Py:   f"{1234567:,}"
来源：http://ruw.sufxvd.cn

PHP:  number_format(1234567);
来源：http://bqp.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kos.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ury.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mst.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqy.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ghv.yj20258.top

C#:   1234567.ToString("N0")
来源：http://day.yongpay.top

[E17] 首字母大写
来源：http://maj.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hvv.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wtr.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://msg.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljk.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://psw.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rod.yfazqb.com

Ruby: s.capitalize
来源：http://uzo.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://elr.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://tgz.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nhd.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yvu.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uwk.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nyl.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lds.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sum.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvo.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://luv.hammf.cn

[E19] 多行文本按行拆分
来源：http://gdo.vehdjk.com

Py:   s.splitlines()
来源：http://syn.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nwi.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://kqt.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://qhc.xziqi.cn

Java: s.lines().toList()
来源：http://oen.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://jcz.ydzc1.top

Ruby: s.lines
来源：http://hvw.cqqwz.cn

C#:   s.Split('\n')
来源：http://sbu.tanke756.top

[E20] 判断字符串是否为空
来源：http://max.sxryk.cn

Py:   if not s:
来源：http://ize.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ycr.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zgw.9152youxi.cn

TS:   if (s === "") {}
来源：http://orp.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://sjj.uphjek.com

Go:   if s == "" {}
来源：http://llp.gogol.net.cn

Ruby: if s.empty?
来源：http://gnw.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hyf.hnqzz.top

[E21] 超长截断加省略号
来源：http://vun.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dez.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gms.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmq.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hvy.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vqn.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://yhe.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xlw.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hmy.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://zfp.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://szq.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bss.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://egy.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://szy.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gbw.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bpj.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://snc.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ens.zhoulong.xyz

================================================================================
来源：http://lir.svipenyu.cn

F. 文件与目录
来源：http://yar.gaohongyu789.top

================================================================================
来源：http://aoz.shzxlz.cn

[F01] 读取整个文件
来源：http://dfl.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vds.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://spr.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gol.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vlm.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qqy.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://udu.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://fov.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://aye.zhoulong.xyz

[F02] 逐行读取文件
来源：http://mvi.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eji.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://avi.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwz.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dad.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://irv.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://neo.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sxq.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rsa.meibo888.top

[F03] 写入文件（覆盖）
来源：http://hon.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wof.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zhr.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jrn.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npu.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gxj.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pag.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://yxw.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hic.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://hnv.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vkh.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gvl.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohk.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pyk.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://umw.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pft.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hic.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lhn.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://ltt.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pdb.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://nrt.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://mwx.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://vud.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aip.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bsf.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://zhi.uphjek.com

C#:   File.Exists("a.txt")
来源：http://gww.xuetiantiany.cn

[F06] 删除文件
来源：http://tsp.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://zto.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://raa.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mqg.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rqo.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ryx.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://vmz.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://glj.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://tcx.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://slh.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://scm.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xhd.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fpv.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kvp.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ixg.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ijz.yangfankeji.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://erm.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jnf.sxryk.cn

[F08] 遍历目录
来源：http://ilr.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qvt.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hjb.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://ytx.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://upg.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mzq.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zur.fktsv.cn

Ruby: Dir.children("dir")
来源：http://qms.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://eoe.gogol.net.cn

[F09] 获取文件大小
来源：http://fro.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://duq.jianghu66.top

PHP:  filesize("a.txt");
来源：http://qqr.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://rsw.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://vyw.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://zfm.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gim.meibo888.top

Ruby: File.size("a.txt")
来源：http://pjy.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://oxi.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://jcr.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://scs.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cma.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iqc.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://qxj.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ogg.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zbf.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kdg.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://csl.cdnleiting.top

[F11] 复制与移动文件
来源：http://iwt.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kfy.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fjh.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aas.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://avf.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dpj.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://glk.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uxb.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lcd.jinqigfzy.top

[F12] CSV 读写
来源：http://aln.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://icq.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lty.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fpn.zdqjudy.top

TS:   // 同上
来源：http://xnf.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ovr.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fyr.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eoj.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ein.316326.xyz

================================================================================
来源：http://vci.ybcxt.top

G. 面向对象
来源：http://jcy.guannengcc.top

================================================================================
来源：http://uno.yonumen.top

[G01] 定义类
来源：http://ctw.shzxlz.cn

Py:   class User: pass
来源：http://xgx.guannengcc.top

PHP:  class User {}
来源：http://sdp.wangdashe.top

JS:   class User {}
来源：http://fps.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://wgu.yfazqb.com

Java: class User {}
来源：http://hez.ppjwa.cn

Go:   type User struct { Name string }
来源：http://tlq.shanyushiyangkeji.top

Ruby: class User; end
来源：http://lgb.hammf.cn

C#:   class User {}
来源：http://avd.vqdsnc.cn

[G02] 构造函数
来源：http://gmb.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://vip.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://hry.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://wye.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://zff.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://rpn.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ink.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://adc.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://dnl.tarul.cn

[G03] 实例属性
来源：http://laz.snrcjt.cn

Py:   self.name = "x"
来源：http://lqt.zhixingplan.top

PHP:  public string $name = "x";
来源：http://rua.meibo888.top

JS:   this.name = "x";
来源：http://clp.cqqwz.cn

TS:   name: string = "x";
来源：http://kvh.zhixingplan.top

Java: private String name;
来源：http://csp.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fkq.tianlin.xyz

Ruby: @name = "x"
来源：http://twi.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://cux.jinqigufen.top

[G04] 定义方法
来源：http://ete.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://vox.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://skq.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://awf.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://xvc.jqgfzy.top

Java: String greet() { return name; }
来源：http://atb.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://avq.hcnkem.com

Ruby: def greet; @name; end
来源：http://awv.yj20258888.top

C#:   public string Greet() => Name;
来源：http://cje.chenzaomai.com

[G05] 继承
来源：http://pik.guannengcc.top

Py:   class Admin(User): pass
来源：http://nkq.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://ekj.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://llh.dashuyun.cn

TS:   class Admin extends User {}
来源：http://fmn.yuanzhike.top

Java: class Admin extends User {}
来源：http://ynr.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uqh.ydzc1.top

Ruby: class Admin < User; end
来源：http://nxe.yj202588.top

C#:   class Admin : User {}
来源：http://hrm.pycfn.com

[G06] 重写方法
来源：http://ptp.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://wwn.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ico.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://luu.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://lhd.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://zlu.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bxq.pycfn.com

Ruby: def greet; "admin"; end
来源：http://enf.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://tot.aizwys.cn

[G07] 调用父类方法
来源：http://uga.yongpay.top

Py:   super().greet()
来源：http://hll.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://ndd.redwolf501.top

JS:   super.greet();
来源：http://biu.sweek.top

TS:   super.greet();
来源：http://qqa.sjlbkw.cn

Java: super.greet();
来源：http://zan.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vfi.ehwqpu.com

Ruby: super
来源：http://dzh.yfazqb.com

C#:   base.Greet();
来源：http://vaw.ydjk.org.cn

[G08] 静态方法与属性
来源：http://ctn.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ygw.jqgufenzy.top

PHP:  public static function f() {}
来源：http://nnp.hesvh.cn

JS:   static f() {}
来源：http://eel.zdqjudy.top

TS:   static f(): void {}
来源：http://hyb.epnwcf.com

Java: static void f() {}
来源：http://ckk.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://snk.aibaodan.cn

Ruby: def self.f; end
来源：http://xbg.quarkkingdee.top

C#:   public static void F() {}
来源：http://jvr.tian-w.cn

[G09] 接口 / 抽象类
来源：http://was.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://yfb.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://tva.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zwr.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://zap.cashguo.top


<!-- 参考信息 -->