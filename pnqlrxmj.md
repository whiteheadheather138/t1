代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mkw.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yqa.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://dgm.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://qnn.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xzz.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pfp.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://jkb.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rho.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://ztx.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lgd.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ysl.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://yok.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://ddi.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://wzn.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://xhf.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gpu.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gdl.andypj.xyz

[E11] 反转字符串
来源：http://eqi.jinqigfzy.top

Py:   s[::-1]
来源：http://wfd.kuanghao11.cn

PHP:  strrev($s);
来源：http://nyf.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://xcy.yongpay.top

TS:   [...s].reverse().join("")
来源：http://zhk.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lvo.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://qfm.hnxiangtu.top

Ruby: s.reverse
来源：http://cqh.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://hcj.yfazqb.com

[E12] 统计某字符出现次数
来源：http://nfu.yonumen.top

Py:   s.count("a")
来源：http://pxx.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://jod.xuanzx.com

JS:   s.split("a").length - 1
来源：http://utg.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://jjh.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qfy.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://ino.ydzc1.top

Ruby: s.count("a")
来源：http://srm.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://kht.xuanzx.com

[E13] 逐字符遍历
来源：http://jrz.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://vhb.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://anx.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fvt.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://smp.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lme.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nob.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gtc.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qcw.daxiang520.top

[E14] URL 编码与 Base64
来源：http://wfe.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bxt.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mla.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pwk.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sma.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vtf.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jgj.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bjv.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ibm.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://jgv.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://dzi.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jdb.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kcc.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jxi.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ktv.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qvw.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cyx.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://did.hongshengwenyu.top

[E16] 数字千分位
来源：http://gdd.hammf.cn

Py:   f"{1234567:,}"
来源：http://yie.c1oappe.top

PHP:  number_format(1234567);
来源：http://hrd.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://yhy.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://iyc.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://omd.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jfr.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ynt.meibo888.top

C#:   1234567.ToString("N0")
来源：http://lda.hnqzz.top

[E17] 首字母大写
来源：http://rjy.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ayc.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vnh.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcz.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wcg.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dvh.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fay.iojbl.cn

Ruby: s.capitalize
来源：http://dzx.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qgy.cheryme.top

[E18] 模板占位符替换
来源：http://xdc.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rgx.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://akx.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://unz.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://xrd.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ovc.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://snb.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kgo.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jtc.shuidangran.top

[E19] 多行文本按行拆分
来源：http://rag.ppjwa.cn

Py:   s.splitlines()
来源：http://bbs.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eox.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://luv.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://pzz.guowangkeji.top

Java: s.lines().toList()
来源：http://vmy.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://vmd.daria6918.cn

Ruby: s.lines
来源：http://fvq.hnqzz.top

C#:   s.Split('\n')
来源：http://alz.andypj.xyz

[E20] 判断字符串是否为空
来源：http://ogw.0kj1m.cn

Py:   if not s:
来源：http://mby.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rpi.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cxa.cqqwz.cn

TS:   if (s === "") {}
来源：http://agy.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://nkt.ctjpmb.com

Go:   if s == "" {}
来源：http://nex.yuxming.cn

Ruby: if s.empty?
来源：http://pat.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eun.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://hlq.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yij.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ukn.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tql.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjv.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dbs.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://aok.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bwv.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xpi.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://oqh.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yzc.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sch.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dho.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yhr.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ypu.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://frt.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://nhn.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ual.yueranfly.top

================================================================================
来源：http://cvd.uphjek.com

F. 文件与目录
来源：http://txx.jiagoushi.top

================================================================================
来源：http://dkt.yj20258.top

[F01] 读取整个文件
来源：http://jxq.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://god.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://ird.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://use.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mhn.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lob.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://edv.havefunace.top

Ruby: File.read("a.txt")
来源：http://ram.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://bwz.xinyue.icu

[F02] 逐行读取文件
来源：http://sxj.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ewb.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qpg.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sqo.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lxv.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pmg.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qcu.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zcb.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wtt.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://ukn.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fcs.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yog.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wqx.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vul.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nyl.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iqw.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://ztv.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://upp.bbcook.cn

[F04] 追加写入文件
来源：http://qrq.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vvi.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jlg.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://njj.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vng.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tfc.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jea.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rjp.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fty.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://jwq.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lxr.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://jqo.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://nvi.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://jkh.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bod.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lyo.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://jrk.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://jnl.cheryme.top

[F06] 删除文件
来源：http://zrp.mhx1999.top

Py:   os.remove("a.txt")
来源：http://qvy.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://xsy.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ghj.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cdv.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jzs.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://ucf.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://geo.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://hpv.havefunace.top

[F07] 创建目录（含多级）
来源：http://fzd.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kkl.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hyj.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://utd.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ern.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xua.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xgy.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zzd.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vyr.gogol.net.cn

[F08] 遍历目录
来源：http://ekr.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmm.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bms.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://zvp.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://ykm.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mjt.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qoy.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://ymz.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://vef.ppjwa.cn

[F09] 获取文件大小
来源：http://anm.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://baa.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://wwr.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://sdw.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://wxx.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sya.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fat.gzhubu.top

Ruby: File.size("a.txt")
来源：http://aca.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://efo.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://gux.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yay.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oeo.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uou.daria6918.cn

TS:   path.extname("a.txt")
来源：http://hvb.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ofb.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nat.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://szb.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qul.hfpthk.cn

[F11] 复制与移动文件
来源：http://eaq.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rzp.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cid.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqj.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kcx.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fet.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmb.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gfd.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bor.shangyingyoupin.top

[F12] CSV 读写
来源：http://kgz.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jmi.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hlu.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tob.uphjek.com

TS:   // 同上
来源：http://jgm.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aee.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wdn.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fzb.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://run.yj20258.top

================================================================================
来源：http://ill.daxiang520.top

G. 面向对象
来源：http://yrn.daxiang520.top

================================================================================
来源：http://tya.bjfxy.top

[G01] 定义类
来源：http://wef.hongshengwenyu.top

Py:   class User: pass
来源：http://fbh.cqqwz.cn

PHP:  class User {}
来源：http://ouo.jianghu66.top

JS:   class User {}
来源：http://kne.yongpay.top

TS:   class User { name: string = ""; }
来源：http://muo.fktsv.cn

Java: class User {}
来源：http://con.svipenyu.cn

Go:   type User struct { Name string }
来源：http://oia.xuetiantiany.cn

Ruby: class User; end
来源：http://tcw.vehdjk.com

C#:   class User {}
来源：http://mmf.sufxvd.cn

[G02] 构造函数
来源：http://hxj.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://zfe.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://jmh.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://jmh.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://gat.sweek.top

Java: User(String name) { this.name = name; }
来源：http://egj.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ytw.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://gjw.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://dvs.zdbjq.cn

[G03] 实例属性
来源：http://esn.jqgufenzy.top

Py:   self.name = "x"
来源：http://tyr.shzxlz.cn

PHP:  public string $name = "x";
来源：http://fmp.daria6918.cn

JS:   this.name = "x";
来源：http://qgz.xuanzx.com

TS:   name: string = "x";
来源：http://mnx.jiagoushi.top

Java: private String name;
来源：http://chd.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kdb.uphjek.com

Ruby: @name = "x"
来源：http://oyg.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://fyz.c1oappe.top

[G04] 定义方法
来源：http://iob.gzhubu.top

Py:   def greet(self): return self.name
来源：http://vdw.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://msh.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://bkl.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://ywn.shzxlz.cn

Java: String greet() { return name; }
来源：http://uss.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://okc.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://zte.cucudq.cn

C#:   public string Greet() => Name;
来源：http://heq.mhx1999.top

[G05] 继承
来源：http://hlz.fehbvm.com

Py:   class Admin(User): pass
来源：http://jnh.hnqzz.top

PHP:  class Admin extends User {}
来源：http://clv.tianlin.xyz

JS:   class Admin extends User {}
来源：http://dhu.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://mle.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://gfk.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kod.9152youxi.cn

Ruby: class Admin < User; end
来源：http://fae.316326.xyz

C#:   class Admin : User {}
来源：http://qsk.bbcook.cn

[G06] 重写方法
来源：http://sja.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://inf.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ktr.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://gvf.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://iyg.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://zak.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xhx.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://hxs.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://tgu.guowangkeji.top

[G07] 调用父类方法
来源：http://cja.316326.xyz

Py:   super().greet()
来源：http://qdu.yangfankeji.com

PHP:  parent::greet();
来源：http://rhu.tianlin.xyz

JS:   super.greet();
来源：http://wge.shzxlz.cn

TS:   super.greet();
来源：http://beg.dashuyun.cn

Java: super.greet();
来源：http://tgz.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hob.nanxinkj.top


<!-- 参考信息 -->