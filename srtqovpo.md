代发 wailian999

PHP:  implode(",", $items);
来源：http://otb.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://dxu.daria6918.cn

TS:   items.join(",")
来源：http://zoi.sufxvd.cn

Java: String.join(",", items)
来源：http://viw.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://jns.jinqigfzy.top

Ruby: items.join(",")
来源：http://nvh.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://fid.svipenyu.cn

[E09] 去除所有空白字符
来源：http://anj.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://inm.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gfw.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://igz.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://xuq.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://rwh.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jhd.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://lmr.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://evt.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://xvk.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ppd.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xwk.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://pfe.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://yte.pycfn.com

Java: String.format("%03d", 7)
来源：http://zug.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wyi.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hgd.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mck.wangshuangyany.cn

[E11] 反转字符串
来源：http://mzt.fehbvm.com

Py:   s[::-1]
来源：http://lzb.52xcode.cn

PHP:  strrev($s);
来源：http://fqw.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://oyg.yongpay.top

TS:   [...s].reverse().join("")
来源：http://zvm.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wpn.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mom.zdqjudy.top

Ruby: s.reverse
来源：http://kxb.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://hsg.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://lrl.yuanzhike.top

Py:   s.count("a")
来源：http://xck.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://ugy.yj20258.top

JS:   s.split("a").length - 1
来源：http://xpl.cashguo.top

TS:   s.split("a").length - 1
来源：http://klf.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rbx.uphjek.com

Go:   strings.Count(s, "a")
来源：http://azl.yangfankeji.com

Ruby: s.count("a")
来源：http://ksp.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://hzs.jlsjyb.cn

[E13] 逐字符遍历
来源：http://iza.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://frd.daxiang520.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://axx.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lxf.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qce.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vmz.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pqv.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lkx.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lfl.daria6918.cn

[E14] URL 编码与 Base64
来源：http://zbk.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iuz.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zeo.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zwt.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fan.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wto.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tia.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rfu.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xac.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://cdq.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kna.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yya.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ohl.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://pgl.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yzg.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pzn.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://amx.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tfd.hesvh.cn

[E16] 数字千分位
来源：http://qry.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://xgl.smart0.xyz

PHP:  number_format(1234567);
来源：http://lrv.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gvd.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ucd.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pcc.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oai.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hlu.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://wxn.sjlbkw.cn

[E17] 首字母大写
来源：http://dft.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rxk.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ywh.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zvj.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://utc.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lie.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hll.fengsongda.top

Ruby: s.capitalize
来源：http://cje.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://got.jyoumei.cn

[E18] 模板占位符替换
来源：http://cfb.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lxu.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yvu.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jin.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://okn.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nut.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ltq.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bdr.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pwn.tarul.cn

[E19] 多行文本按行拆分
来源：http://kph.pengpengdd.cyou

Py:   s.splitlines()
来源：http://yrf.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vml.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://cmj.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://yyk.sysykeji.top

Java: s.lines().toList()
来源：http://nes.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://nii.redwolf501.top

Ruby: s.lines
来源：http://xij.ppjwa.cn

C#:   s.Split('\n')
来源：http://pvn.wangdashe.top

[E20] 判断字符串是否为空
来源：http://ihh.ydjk.org.cn

Py:   if not s:
来源：http://lce.iojbl.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ucz.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cbr.jianghu66.top

TS:   if (s === "") {}
来源：http://clx.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://gul.sxryk.cn

Go:   if s == "" {}
来源：http://kti.jqgfzy.top

Ruby: if s.empty?
来源：http://rrl.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nsv.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://ddj.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sfr.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://euc.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lzh.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mbg.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://obw.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://fij.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://psx.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://got.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://kvk.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bwe.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://soi.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pgo.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tbd.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wyf.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yaa.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://mas.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vrx.jiagoushi.top

================================================================================
来源：http://gxs.ctjpmb.com

F. 文件与目录
来源：http://qdh.jlsjyb.cn

================================================================================
来源：http://frz.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://tgs.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lgh.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://qeu.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vjd.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dgd.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wwd.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://boj.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://bpk.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://ifw.jinqigufen.top

[F02] 逐行读取文件
来源：http://bbo.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://udk.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://avn.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kwc.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvr.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qfr.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://avi.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kti.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lck.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://vzk.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tig.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kmv.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eep.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wna.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ojf.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://siw.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://gkw.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zvh.yvedp.cn

[F04] 追加写入文件
来源：http://yrh.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ilp.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lfk.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xpj.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfq.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vbl.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rmc.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ici.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://roh.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://muz.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gai.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://vfm.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://zgq.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://kok.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://knq.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fvx.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://pqj.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://hko.zhongyouzk.top

[F06] 删除文件
来源：http://qpo.c1oappe.top

Py:   os.remove("a.txt")
来源：http://nyk.fengsongda.top

PHP:  unlink("a.txt");
来源：http://lny.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tzl.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://agw.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vle.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://ebm.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://hdm.cashguo.top

C#:   File.Delete("a.txt");
来源：http://klt.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://qae.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qqg.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cpz.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vht.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ada.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cth.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qck.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dqe.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vyd.ivvv.top

[F08] 遍历目录
来源：http://iak.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kdq.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qgs.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://xcj.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://stt.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lig.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bwn.mhx1999.top

Ruby: Dir.children("dir")
来源：http://iqa.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://fem.meibo888.top

[F09] 获取文件大小
来源：http://flj.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://fdb.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://hdz.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://lqq.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://rat.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://pib.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ozo.tanke756.top

Ruby: File.size("a.txt")
来源：http://rxf.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://zdy.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://tho.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lnp.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vnb.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fmo.pycfn.com

TS:   path.extname("a.txt")
来源：http://tor.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://irj.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fqh.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tld.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qkz.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://sjv.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ctd.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://six.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://irt.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://agc.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fse.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nif.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://muu.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nky.jianghu66.top

[F12] CSV 读写
来源：http://sdo.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tle.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fgu.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqn.xylfe.cn

TS:   // 同上
来源：http://prp.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ekl.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ivt.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gqm.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rus.aizwys.cn

================================================================================
来源：http://qqn.cucudq.cn

G. 面向对象
来源：http://opl.andypj.xyz

================================================================================
来源：http://nwa.jianghu66.top

[G01] 定义类
来源：http://sqd.fzhhl.top

Py:   class User: pass
来源：http://pzv.aizwys.cn

PHP:  class User {}
来源：http://ngz.gotoacloud.top

JS:   class User {}
来源：http://kga.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://qjr.ydzc1.top

Java: class User {}
来源：http://aek.nwbrower.top

Go:   type User struct { Name string }
来源：http://tbf.tianlin.xyz

Ruby: class User; end
来源：http://qko.fengsongda.top

C#:   class User {}
来源：http://dre.vqdsnc.cn

[G02] 构造函数
来源：http://gvl.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://pak.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://zed.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://bxd.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://zph.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://pea.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gyp.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://iva.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://not.sysykeji.top

[G03] 实例属性
来源：http://qup.tarul.cn

Py:   self.name = "x"
来源：http://ujt.sysykeji.top

PHP:  public string $name = "x";
来源：http://thz.birdmap.top

JS:   this.name = "x";
来源：http://tfe.zhoulong.xyz

TS:   name: string = "x";
来源：http://gqi.316326.xyz

Java: private String name;
来源：http://wuv.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qlf.shzxlz.cn

Ruby: @name = "x"
来源：http://frb.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://eov.shuidangran.top

[G04] 定义方法
来源：http://uta.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://evh.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sel.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://zrh.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://rjv.hywenlv.cn

Java: String greet() { return name; }
来源：http://jzn.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://imy.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://vtk.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://dqo.fzhhl.top

[G05] 继承
来源：http://ndv.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://rbl.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://jpq.hysaishi.cn

JS:   class Admin extends User {}
来源：http://tln.shuidangran.top

TS:   class Admin extends User {}
来源：http://khs.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://xmd.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hys.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://avn.jianghu66.top

C#:   class Admin : User {}
来源：http://wfu.zhoulong.xyz

[G06] 重写方法
来源：http://jng.meibo888.top

Py:   def greet(self): return "admin"
来源：http://uis.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ihw.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://yko.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://tvu.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://qzx.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pcy.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://sdn.hcnkem.com


<!-- 参考信息 -->