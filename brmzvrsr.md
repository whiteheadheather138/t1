代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://pnn.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uuz.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://etn.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tbe.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://xnp.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mds.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oji.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://epr.sweek.top

TS:   "7".padStart(3, "0")
来源：http://ima.mhx1999.top

Java: String.format("%03d", 7)
来源：http://mdq.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://kpn.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxi.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vxy.aibaodan.cn

[E11] 反转字符串
来源：http://zfb.vqdsnc.cn

Py:   s[::-1]
来源：http://iix.jianghu66.top

PHP:  strrev($s);
来源：http://xbp.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://dox.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://dfq.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sxd.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rfj.sjlbkw.cn

Ruby: s.reverse
来源：http://evq.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://odf.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://lrn.birdmap.top

Py:   s.count("a")
来源：http://soj.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://eoa.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://mbx.yonumen.top

TS:   s.split("a").length - 1
来源：http://mmt.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vit.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://wnz.zhoulong.xyz

Ruby: s.count("a")
来源：http://zjh.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://jkx.zhixingplan.top

[E13] 逐字符遍历
来源：http://fbb.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://xkw.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://geo.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://jvi.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jwc.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wkc.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cqk.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://upk.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ssy.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://urz.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lme.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://xal.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kuy.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bed.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ixz.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://grs.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://otn.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://orr.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://jlz.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tqf.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xhx.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gcx.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nyr.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ruj.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oaf.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hzg.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qtz.hnqzz.top

[E16] 数字千分位
来源：http://ncc.jianghu66.top

Py:   f"{1234567:,}"
来源：http://wmi.zdbjq.cn

PHP:  number_format(1234567);
来源：http://aaq.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mzw.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://iod.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lzi.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://biu.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ret.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://kbh.yvedp.cn

[E17] 首字母大写
来源：http://qhi.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blo.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://gyl.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcm.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umz.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dbp.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mca.shangyingyoupin.top

Ruby: s.capitalize
来源：http://ksy.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lms.yfazqb.com

[E18] 模板占位符替换
来源：http://zkp.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jlf.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wnp.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jmj.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fll.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ktd.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqx.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wnf.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fqv.gzhubu.top

[E19] 多行文本按行拆分
来源：http://wof.gzhubu.top

Py:   s.splitlines()
来源：http://zaz.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vkf.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://jxn.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://pho.aibaodan.cn

Java: s.lines().toList()
来源：http://rpb.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://ksp.gotoacloud.top

Ruby: s.lines
来源：http://zil.hammf.cn

C#:   s.Split('\n')
来源：http://yev.52xcode.cn

[E20] 判断字符串是否为空
来源：http://tap.vehdjk.com

Py:   if not s:
来源：http://ijy.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://grg.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rlp.yvedp.cn

TS:   if (s === "") {}
来源：http://due.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://hdl.hywenlv.cn

Go:   if s == "" {}
来源：http://hvs.yfazqb.com

Ruby: if s.empty?
来源：http://ebp.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hjh.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://ipc.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kuu.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yuz.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://svf.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dre.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jny.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://oin.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xlb.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pnv.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://dnw.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hdu.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbf.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eio.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jaw.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kxc.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://twl.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://lga.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dgi.sufxvd.cn

================================================================================
来源：http://aev.xingfuxueyuan.xyz

F. 文件与目录
来源：http://qcv.wangdashe.top

================================================================================
来源：http://jgd.ybcxt.top

[F01] 读取整个文件
来源：http://iwu.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rwp.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://ggl.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ujm.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eth.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uim.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ixu.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://drw.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://cpa.zdqjudy.top

[F02] 逐行读取文件
来源：http://nfb.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://adm.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://igr.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://erd.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://avi.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qke.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zjr.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://axo.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jhc.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://oyq.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fnj.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kib.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://noi.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fph.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fif.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pkj.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://tpq.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iga.yj202588.top

[F04] 追加写入文件
来源：http://zxh.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tpz.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ghk.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://beo.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uee.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://laf.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nyv.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://byg.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tjd.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://kzg.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ryj.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://zie.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://xvx.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://hkt.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yyr.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rvo.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://sox.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://rbg.snrcjt.cn

[F06] 删除文件
来源：http://piq.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://eru.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://qxh.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dlh.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://cyt.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://shj.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://qbk.ivvv.top

Ruby: File.delete("a.txt")
来源：http://hqh.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://ogy.yueranfly.top

[F07] 创建目录（含多级）
来源：http://emq.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hty.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lcj.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bul.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hvv.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mmm.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fpy.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mvk.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pdr.zhiwuduotai.top

[F08] 遍历目录
来源：http://lms.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mtg.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jrb.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://uhv.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://rba.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ren.wangdashe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qan.havefunace.top

Ruby: Dir.children("dir")
来源：http://pca.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://frr.ybcxt.top

[F09] 获取文件大小
来源：http://ywh.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://xhw.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://uew.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://kkh.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://ygz.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://xjv.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ljb.andypj.xyz

Ruby: File.size("a.txt")
来源：http://owh.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://ude.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://xqw.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://urk.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjt.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pke.yj20258888.top

TS:   path.extname("a.txt")
来源：http://ozk.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mgy.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://otm.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ent.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lay.guannengcc.top

[F11] 复制与移动文件
来源：http://mel.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ivf.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tiz.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ory.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqo.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uzf.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://isx.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xzz.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rjm.mhx1999.top

[F12] CSV 读写
来源：http://lsd.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gib.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yeu.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://psu.tanke756.top

TS:   // 同上
来源：http://bay.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hdl.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bzw.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hkv.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tbk.nanxuanxn.top

================================================================================
来源：http://zap.dashuyun.cn

G. 面向对象
来源：http://rqb.zhengqikj.top

================================================================================
来源：http://gbb.shangyingyoupin.top

[G01] 定义类
来源：http://dyp.tarul.cn

Py:   class User: pass
来源：http://gix.ivvv.top

PHP:  class User {}
来源：http://pie.yj20258.top

JS:   class User {}
来源：http://iyn.pycfn.com

TS:   class User { name: string = ""; }
来源：http://ato.sufxvd.cn

Java: class User {}
来源：http://xkn.bjfxy.top

Go:   type User struct { Name string }
来源：http://qha.iojbl.cn

Ruby: class User; end
来源：http://cab.birdmap.top

C#:   class User {}
来源：http://hqu.fktsv.cn

[G02] 构造函数
来源：http://rhc.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://rsy.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://oye.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://ejr.yj20258.top

TS:   constructor(public name: string) {}
来源：http://zzs.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://qbb.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xzx.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://yid.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://pcl.zhongyouzk.top

[G03] 实例属性
来源：http://ckp.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://itv.9152youxi.cn

PHP:  public string $name = "x";
来源：http://zhl.nanxinkj.top

JS:   this.name = "x";
来源：http://zpg.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://hpw.guannengcc.top

Java: private String name;
来源：http://itl.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mrf.xinyue.icu

Ruby: @name = "x"
来源：http://hbc.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://dgk.nwbrower.top

[G04] 定义方法
来源：http://kil.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://hzf.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://hqu.pycfn.com

JS:   greet() { return this.name; }
来源：http://ozj.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://mji.ydzc1.top

Java: String greet() { return name; }
来源：http://yyn.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dju.cashguo.top

Ruby: def greet; @name; end
来源：http://kqw.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://res.jyoumei.cn

[G05] 继承
来源：http://gam.jiagoushi.top

Py:   class Admin(User): pass
来源：http://txf.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://esy.iojbl.cn

JS:   class Admin extends User {}
来源：http://gwy.bbcook.cn

TS:   class Admin extends User {}
来源：http://yre.ehwqpu.com

Java: class Admin extends User {}
来源：http://dlc.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://csq.yj202588.top

Ruby: class Admin < User; end
来源：http://dsy.hammf.cn

C#:   class Admin : User {}
来源：http://srd.shuidangran.top

[G06] 重写方法
来源：http://fiu.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://jyf.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tpl.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://lni.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://kmg.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://upi.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gym.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://rdg.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://xdm.bbcook.cn

[G07] 调用父类方法
来源：http://ftw.quarkkingdee.top

Py:   super().greet()
来源：http://jiv.guowangkeji.top

PHP:  parent::greet();
来源：http://xcc.kuanghao11.cn

JS:   super.greet();
来源：http://ili.fehbvm.com

TS:   super.greet();
来源：http://ccf.shzxlz.cn

Java: super.greet();
来源：http://dmd.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nmn.yonumen.top

Ruby: super
来源：http://obp.shanyushiyangtech.top

C#:   base.Greet();
来源：http://igs.redwolf501.top

[G08] 静态方法与属性
来源：http://gqb.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hfw.wangshuangyany.cn


<!-- 参考信息 -->