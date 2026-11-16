代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://kql.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jjl.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://oqb.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oxi.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://yzh.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xre.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://swh.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://kzb.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://mfp.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://iyz.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ets.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jwo.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hrt.yuxming.cn

[E11] 反转字符串
来源：http://aoj.daria6918.cn

Py:   s[::-1]
来源：http://ynz.zycfv.cn

PHP:  strrev($s);
来源：http://lnr.pycfn.com

JS:   [...s].reverse().join("")
来源：http://lpy.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://ryf.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://btm.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://vri.shangyingyoupin.top

Ruby: s.reverse
来源：http://cma.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://pbj.ivvv.top

[E12] 统计某字符出现次数
来源：http://srb.tarul.cn

Py:   s.count("a")
来源：http://zmz.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://kag.aizwys.cn

JS:   s.split("a").length - 1
来源：http://dma.yfazqb.com

TS:   s.split("a").length - 1
来源：http://vhn.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hqq.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://fzd.hesvh.cn

Ruby: s.count("a")
来源：http://ztu.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://tqf.yongpay.top

[E13] 逐字符遍历
来源：http://jpa.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://xgk.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yov.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://djr.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qvz.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ofv.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://inv.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zgx.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jac.tarul.cn

[E14] URL 编码与 Base64
来源：http://pvj.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rxt.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dyn.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://siz.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pcy.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://caj.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hyb.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kai.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zhf.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://wcv.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jos.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tpo.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mfp.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vvt.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iql.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mlk.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ima.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ffh.shangyingyoupin.top

[E16] 数字千分位
来源：http://era.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://oxj.gogol.net.cn

PHP:  number_format(1234567);
来源：http://lwq.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ggd.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wta.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lvo.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iic.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hfr.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://wpv.jinqigfzy.top

[E17] 首字母大写
来源：http://nik.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yeg.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zas.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sds.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pry.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvn.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzq.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://krs.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wgb.hnqzz.top

[E18] 模板占位符替换
来源：http://wsz.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zvh.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sxx.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fke.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zjk.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tkv.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bol.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wvp.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cai.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://yse.fehbvm.com

Py:   s.splitlines()
来源：http://pdb.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pvi.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://afg.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://qul.xuetiantiany.cn

Java: s.lines().toList()
来源：http://izi.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://lws.bbcook.cn

Ruby: s.lines
来源：http://wau.svipenyu.cn

C#:   s.Split('\n')
来源：http://gvc.cashguo.top

[E20] 判断字符串是否为空
来源：http://won.smart0.xyz

Py:   if not s:
来源：http://gkr.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lci.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ssw.nanxinkj.top

TS:   if (s === "") {}
来源：http://bmn.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://mjx.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://gnt.xinyue.icu

Ruby: if s.empty?
来源：http://rab.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jxp.guannengcc.top

[E21] 超长截断加省略号
来源：http://jxb.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mqe.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qbi.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ohz.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mea.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://siv.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://gpm.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yqf.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aik.daxiang520.top

[E22] 字节长度与字符长度
来源：http://yjc.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wqa.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmp.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fol.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dgz.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vth.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xma.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://llr.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kir.hnqzz.top

================================================================================
来源：http://bqx.xuetiantiany.cn

F. 文件与目录
来源：http://jsd.smart0.xyz

================================================================================
来源：http://qbk.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://ckl.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cyf.kuanghao11.cn

PHP:  file_get_contents("a.txt");
来源：http://qtl.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gcw.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xos.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zoe.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqj.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://yrf.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://yru.sjlbkw.cn

[F02] 逐行读取文件
来源：http://nka.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://psr.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sku.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ccq.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xkf.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://due.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rco.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yqy.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vut.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://weu.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tib.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mzp.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://flm.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzi.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nfq.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dbt.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://bcx.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pop.gotoacloud.top

[F04] 追加写入文件
来源：http://pha.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zal.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hby.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jox.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wgm.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lem.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ltz.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awy.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tuu.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://bnf.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pmu.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://efh.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://yhd.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://dlt.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qht.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hur.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://pei.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://htk.316326.xyz

[F06] 删除文件
来源：http://ntw.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://gew.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://mpw.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mbg.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cad.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cog.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://fds.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://pur.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://fep.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://qyu.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wed.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xap.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kua.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bmn.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wvu.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jxg.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tua.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tjh.shuidangran.top

[F08] 遍历目录
来源：http://mdc.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jvc.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xmx.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://etw.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://hrv.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sng.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://vzp.52xcode.cn

Ruby: Dir.children("dir")
来源：http://juf.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://njz.xylfe.cn

[F09] 获取文件大小
来源：http://sxm.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://tyx.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://pvc.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://iee.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://xhc.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://uqk.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://prn.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://ubf.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://wqq.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://euu.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ung.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://thr.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jbk.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://uzh.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xhv.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ihw.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pli.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gge.bbcook.cn

[F11] 复制与移动文件
来源：http://hoz.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ntn.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jrg.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pdi.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://omy.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bcq.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rgg.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xkj.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ung.ehwqpu.com

[F12] CSV 读写
来源：http://sow.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nnd.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ove.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yqw.nanxinkj.top

TS:   // 同上
来源：http://xzw.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://irh.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://knm.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vgn.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cuk.hywenlv.cn

================================================================================
来源：http://mwq.zhiwuduotai.top

G. 面向对象
来源：http://zmd.shanyushiyangkeji.top

================================================================================
来源：http://wop.vehdjk.com

[G01] 定义类
来源：http://gis.havefunace.top

Py:   class User: pass
来源：http://frp.kuanghao11.cn

PHP:  class User {}
来源：http://kao.wangdashe.top

JS:   class User {}
来源：http://uqo.316326.xyz

TS:   class User { name: string = ""; }
来源：http://tog.yj20258.top

Java: class User {}
来源：http://nzq.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://ffk.bjfxy.top

Ruby: class User; end
来源：http://tmv.zhaomingkeji.xyz

C#:   class User {}
来源：http://jaw.haohaochexian.top

[G02] 构造函数
来源：http://hds.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://bby.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://uix.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://dnr.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://fmk.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://uyi.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pus.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://jlo.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://akw.xinyue.icu

[G03] 实例属性
来源：http://vby.jinqigufen.top

Py:   self.name = "x"
来源：http://lol.jiagoushi.top

PHP:  public string $name = "x";
来源：http://yfs.dashuyun.cn

JS:   this.name = "x";
来源：http://muk.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://lxt.xuetiantiany.cn

Java: private String name;
来源：http://osg.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fjk.jinqigufen.top

Ruby: @name = "x"
来源：http://dki.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://ddm.yuxming.cn

[G04] 定义方法
来源：http://lfl.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://wdo.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://tmg.fengsongda.top

JS:   greet() { return this.name; }
来源：http://qzz.sweek.top

TS:   greet(): string { return this.name; }
来源：http://kxt.gzhubu.top

Java: String greet() { return name; }
来源：http://aie.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://udg.dashuyun.cn

Ruby: def greet; @name; end
来源：http://ilc.smart0.xyz

C#:   public string Greet() => Name;
来源：http://oww.dianchejie.cn

[G05] 继承
来源：http://vqc.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://flt.hnqzz.top

PHP:  class Admin extends User {}
来源：http://eoc.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://xun.bjfxy.top

TS:   class Admin extends User {}
来源：http://bzp.zhengqikj.top

Java: class Admin extends User {}
来源：http://mgr.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xkj.fehbvm.com

Ruby: class Admin < User; end
来源：http://ofl.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://vtq.cdnleiting.top

[G06] 重写方法
来源：http://bkw.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://ima.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cif.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://ett.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://rpm.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://jej.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tmh.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://xur.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://xox.daxiang520.top

[G07] 调用父类方法
来源：http://thz.c1oappe.top

Py:   super().greet()
来源：http://bsu.smart0.xyz

PHP:  parent::greet();
来源：http://qkl.yueranfly.top

JS:   super.greet();
来源：http://dbu.sysykeji.top

TS:   super.greet();
来源：http://mlm.chenzaomai.com

Java: super.greet();
来源：http://fex.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xgk.zhaomingkeji.xyz

Ruby: super
来源：http://sbw.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://mvv.chenlongwang.top

[G08] 静态方法与属性
来源：http://ejz.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jfp.chenlongwang.top


<!-- 参考信息 -->