代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://edb.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hid.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://ybm.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://ckn.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://mnm.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pus.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yet.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jvr.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://rdz.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qmo.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lip.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://nti.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://prf.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://gsy.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ruc.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aka.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kik.cqqwz.cn

[E11] 反转字符串
来源：http://ruu.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://fzb.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://vly.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://zdk.yonumen.top

TS:   [...s].reverse().join("")
来源：http://vxl.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sdl.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yhk.ehwqpu.com

Ruby: s.reverse
来源：http://cxo.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://qap.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://ozt.zhengqikj.top

Py:   s.count("a")
来源：http://bcl.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://wqu.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://jzz.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://wny.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oha.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://bbq.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://kde.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://eau.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://mgb.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://jfp.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wmu.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://osr.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lge.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bow.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eta.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iqp.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fqi.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://xzm.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://num.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://von.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yni.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ktt.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xfs.yvedp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gai.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://szn.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wny.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://iwl.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://tce.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vfy.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ylk.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://khh.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ceu.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://meg.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cmv.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lif.wangdashe.top

[E16] 数字千分位
来源：http://whq.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://vkr.ehwqpu.com

PHP:  number_format(1234567);
来源：http://qos.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mbv.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jic.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ecc.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ibw.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hji.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://jcm.yueranfly.top

[E17] 首字母大写
来源：http://shp.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mtk.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kaa.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://whh.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bja.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zbz.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nah.hammf.cn

Ruby: s.capitalize
来源：http://iwd.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpy.bbcook.cn

[E18] 模板占位符替换
来源：http://yee.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zlj.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oxc.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uxc.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wmk.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ypy.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ekp.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fvc.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jxx.hesvh.cn

[E19] 多行文本按行拆分
来源：http://sib.ydjk.org.cn

Py:   s.splitlines()
来源：http://znq.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hkq.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://ztm.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://kon.tianlin.xyz

Java: s.lines().toList()
来源：http://pln.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://ufn.yangfankeji.com

Ruby: s.lines
来源：http://cat.nwbrower.top

C#:   s.Split('\n')
来源：http://qgl.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://kgh.jinghuilouyu.cn

Py:   if not s:
来源：http://ybb.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://teg.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pfr.ppjwa.cn

TS:   if (s === "") {}
来源：http://iap.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://vjq.shuidangran.top

Go:   if s == "" {}
来源：http://qql.tian-w.cn

Ruby: if s.empty?
来源：http://ahr.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qbi.sweek.top

[E21] 超长截断加省略号
来源：http://ikt.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qnm.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pmp.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzk.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyv.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dhr.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://kfx.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://asn.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xop.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://mxc.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wsu.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://doz.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://woj.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tii.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tqq.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xxb.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://mnh.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pvw.yonumen.top

================================================================================
来源：http://zht.chenzaomai.com

F. 文件与目录
来源：http://mkz.jyoumei.cn

================================================================================
来源：http://yhq.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://tot.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dxn.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://jpj.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oof.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://twg.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vlc.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dhd.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://jhx.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://hva.wangdashe.top

[F02] 逐行读取文件
来源：http://uzh.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qny.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://egs.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ksg.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwd.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ojb.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pya.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rsd.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kvo.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://raa.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tqj.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ohh.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fgx.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbh.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cfo.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kmc.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://lxm.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://erz.zhiwuduotai.top

[F04] 追加写入文件
来源：http://isu.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zxd.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ffz.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://onf.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dqq.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dlt.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rzi.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://osl.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ota.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://atr.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://owg.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://xrt.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://gem.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://rcf.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://htj.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vui.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://yyv.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://xrc.yvedp.cn

[F06] 删除文件
来源：http://lor.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://jhe.havefunace.top

PHP:  unlink("a.txt");
来源：http://qge.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qjv.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://pga.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pxj.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://xmv.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://psp.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://ubz.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://bub.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cfz.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ivd.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uni.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivw.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gle.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rno.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwe.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://siw.snrcjt.cn

[F08] 遍历目录
来源：http://hku.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ldx.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yay.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://gcu.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://tvl.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bow.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://afg.fehbvm.com

Ruby: Dir.children("dir")
来源：http://nnl.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://bqc.daria6918.cn

[F09] 获取文件大小
来源：http://uad.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://acf.sxryk.cn

PHP:  filesize("a.txt");
来源：http://pix.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://ojy.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://hrl.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://urf.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hji.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://ojk.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://evg.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://lme.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yzq.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zwk.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jnh.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://ckh.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rrb.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uwu.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://clt.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://inf.yongpay.top

[F11] 复制与移动文件
来源：http://uhs.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://znr.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cni.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jwq.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nvt.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mjk.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pgv.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xjh.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qbz.yuanzhike.top

[F12] CSV 读写
来源：http://rjx.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bcf.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mpw.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://slt.gzhubu.top

TS:   // 同上
来源：http://vzi.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aty.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://htf.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qzj.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pwk.kuanghao11.cn

================================================================================
来源：http://eyh.cashguo.top

G. 面向对象
来源：http://cec.dashuyun.cn

================================================================================
来源：http://inl.zhongyouzk.top

[G01] 定义类
来源：http://ofd.fehbvm.com

Py:   class User: pass
来源：http://qxr.jinqigfzy.top

PHP:  class User {}
来源：http://lbw.xziqi.cn

JS:   class User {}
来源：http://jou.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://oci.xziqi.cn

Java: class User {}
来源：http://tod.zdbjq.cn

Go:   type User struct { Name string }
来源：http://brf.vqdsnc.cn

Ruby: class User; end
来源：http://jsn.uphjek.com

C#:   class User {}
来源：http://bnb.yvedp.cn

[G02] 构造函数
来源：http://xyv.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://qzn.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://qzp.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://lzu.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://fpr.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://xfg.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lqj.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://abd.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://oqw.yonumen.top

[G03] 实例属性
来源：http://ttw.epnwcf.com

Py:   self.name = "x"
来源：http://tmu.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://lus.pycfn.com

JS:   this.name = "x";
来源：http://tzf.zhiwuduotai.top

TS:   name: string = "x";
来源：http://yvj.jinqigfzy.top

Java: private String name;
来源：http://isg.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hqd.epnwcf.com

Ruby: @name = "x"
来源：http://ufb.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://zdy.ppjwa.cn

[G04] 定义方法
来源：http://nfq.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://wsq.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://oat.52xcode.cn

JS:   greet() { return this.name; }
来源：http://yev.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://ptz.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://rwm.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xzz.vehdjk.com

Ruby: def greet; @name; end
来源：http://qyq.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://fne.xuanzx.com

[G05] 继承
来源：http://tuv.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://kte.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://iag.yuanzhike.top

JS:   class Admin extends User {}
来源：http://fry.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://pid.yvedp.cn

Java: class Admin extends User {}
来源：http://ftl.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bdi.guowangkeji.top

Ruby: class Admin < User; end
来源：http://wsz.shzxlz.cn

C#:   class Admin : User {}
来源：http://gsm.jqgufenzy.top

[G06] 重写方法
来源：http://dob.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://iew.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zws.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://gki.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://cqx.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://dji.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pgn.havefunace.top

Ruby: def greet; "admin"; end
来源：http://lup.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://iqr.vehdjk.com

[G07] 调用父类方法
来源：http://akl.yj20258888.top

Py:   super().greet()
来源：http://asp.shzxlz.cn

PHP:  parent::greet();
来源：http://fac.gaohongyu789.top

JS:   super.greet();
来源：http://okz.sysykeji.top

TS:   super.greet();
来源：http://mmn.feifeiyinyue.top

Java: super.greet();
来源：http://mlq.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dlj.yanxiufei.cn


<!-- 参考信息 -->