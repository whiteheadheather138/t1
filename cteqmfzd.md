代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ucz.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nls.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://cjb.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ddv.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://kgj.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpc.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hob.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://kby.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://fze.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://zvf.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vkq.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kpy.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ads.yuanzhike.top

[E11] 反转字符串
来源：http://enr.chenlongwang.top

Py:   s[::-1]
来源：http://veh.xuetiantiany.cn

PHP:  strrev($s);
来源：http://uuh.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://dgx.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://kjs.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ysl.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zio.316326.xyz

Ruby: s.reverse
来源：http://vrv.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jxa.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://qju.cdnleiting.top

Py:   s.count("a")
来源：http://wmc.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://kxb.xziqi.cn

JS:   s.split("a").length - 1
来源：http://gwq.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://sky.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tzz.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://fsh.hcnkem.com

Ruby: s.count("a")
来源：http://dqh.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://qnj.hcnkem.com

[E13] 逐字符遍历
来源：http://jpy.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://hjj.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vfd.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dsx.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tea.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sdv.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://svx.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wdi.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rky.xuanzx.com

[E14] URL 编码与 Base64
来源：http://hcb.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zeh.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sfl.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xzf.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qyf.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ili.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wds.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sjl.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eet.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://hhh.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://jey.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vgd.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ikt.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tgz.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qdf.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://suw.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tvs.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ajz.aizwys.cn

[E16] 数字千分位
来源：http://xtf.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://sbg.yj202588.top

PHP:  number_format(1234567);
来源：http://yqp.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xod.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cvv.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhk.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://quw.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rum.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://ciy.tanke756.top

[E17] 首字母大写
来源：http://ybv.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://igd.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kks.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://omw.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nsd.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sao.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vnl.0kj1m.cn

Ruby: s.capitalize
来源：http://xog.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwf.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://mpp.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ksn.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ecq.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qbj.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jdy.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://way.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ehj.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xby.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tut.guannengcc.top

[E19] 多行文本按行拆分
来源：http://idf.jqgfzy.top

Py:   s.splitlines()
来源：http://gyt.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iiz.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://foh.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://hpi.tianlin.xyz

Java: s.lines().toList()
来源：http://prs.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://pdp.c1oappe.top

Ruby: s.lines
来源：http://xep.hywenlv.cn

C#:   s.Split('\n')
来源：http://lwv.nwbrower.top

[E20] 判断字符串是否为空
来源：http://gvh.sxryk.cn

Py:   if not s:
来源：http://yzv.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mib.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ijs.vqdsnc.cn

TS:   if (s === "") {}
来源：http://hrj.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://spm.redwolf501.top

Go:   if s == "" {}
来源：http://bna.quarkkingdee.top

Ruby: if s.empty?
来源：http://jbp.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cbw.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://jvl.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hjn.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qbu.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ysa.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xcg.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wjt.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://vxr.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://loj.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vnd.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://rvc.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tqn.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jas.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ftk.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zlj.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://spf.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ahq.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://mwi.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kgr.cucudq.cn

================================================================================
来源：http://aac.yuxming.cn

F. 文件与目录
来源：http://itp.tarul.cn

================================================================================
来源：http://kzh.cashguo.top

[F01] 读取整个文件
来源：http://rog.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rbv.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://qtu.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dmt.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iyp.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nao.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vmd.tanke756.top

Ruby: File.read("a.txt")
来源：http://vrv.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://ues.wangdashe.top

[F02] 逐行读取文件
来源：http://yxe.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npa.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kzg.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhy.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jkg.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lfy.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rbc.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://akr.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zjp.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://bks.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xet.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://euv.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qcy.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kfy.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fix.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ktw.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://lxi.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://odo.birdmap.top

[F04] 追加写入文件
来源：http://fgh.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rie.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pdy.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xqi.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aki.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pgw.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eqv.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dyj.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gti.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://fbc.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wdb.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://qqi.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://oiw.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://mfs.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://kij.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://apv.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://zca.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://qlp.fehbvm.com

[F06] 删除文件
来源：http://xdr.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://gmd.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://lju.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://rfs.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://vbp.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://coa.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://kue.sweek.top

Ruby: File.delete("a.txt")
来源：http://jss.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://voe.shuidangran.top

[F07] 创建目录（含多级）
来源：http://kvw.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://exg.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rrp.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dlq.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lbf.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xzu.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pga.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://udi.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://puk.hysaishi.cn

[F08] 遍历目录
来源：http://ggp.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jyc.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zqy.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://xby.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://vzx.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yup.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://otu.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://nkk.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://ubb.yueranfly.top

[F09] 获取文件大小
来源：http://uxh.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://iia.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://ftm.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://acy.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://xwr.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dpj.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://acj.tanke756.top

Ruby: File.size("a.txt")
来源：http://koj.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://ukw.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://ggd.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ilt.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zhl.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://evy.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://lfc.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tpd.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kic.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://voi.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jjp.yj20258.top

[F11] 复制与移动文件
来源：http://liv.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xig.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iev.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ecx.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://znk.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dty.fzhhl.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tdx.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nrt.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qiu.pycfn.com

[F12] CSV 读写
来源：http://cns.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ohj.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iga.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yux.ydzc1.top

TS:   // 同上
来源：http://zzs.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tpg.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fuo.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://azf.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://zvy.ydzc1.top

================================================================================
来源：http://zfn.chenlongwang.top

G. 面向对象
来源：http://ktm.fehbvm.com

================================================================================
来源：http://zcj.hysaishi.cn

[G01] 定义类
来源：http://jvn.52xcode.cn

Py:   class User: pass
来源：http://mom.chenjidiqi.icu

PHP:  class User {}
来源：http://yyz.daxiang520.top

JS:   class User {}
来源：http://tog.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://wga.zhoulong.xyz

Java: class User {}
来源：http://cjs.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://kvi.yonumen.top

Ruby: class User; end
来源：http://uml.jlsjyb.cn

C#:   class User {}
来源：http://pet.cashguo.top

[G02] 构造函数
来源：http://fed.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://lir.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://xml.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://msf.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://wds.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://yhz.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jwo.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://qee.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://tzo.vehdjk.com

[G03] 实例属性
来源：http://dtd.fengsongda.top

Py:   self.name = "x"
来源：http://juf.zhixingplan.top

PHP:  public string $name = "x";
来源：http://tkr.hnxiangtu.top

JS:   this.name = "x";
来源：http://gyi.hcnkem.com

TS:   name: string = "x";
来源：http://ana.shzxlz.cn

Java: private String name;
来源：http://uyo.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ghq.chenzaomai.com

Ruby: @name = "x"
来源：http://eyx.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://rbg.shzxlz.cn

[G04] 定义方法
来源：http://xmi.sweek.top

Py:   def greet(self): return self.name
来源：http://stk.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://oqn.guannengcc.top

JS:   greet() { return this.name; }
来源：http://ztw.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://zqy.yvedp.cn

Java: String greet() { return name; }
来源：http://jvg.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vhw.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://kub.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://jex.ehwqpu.com

[G05] 继承
来源：http://gsf.yj20258888.top

Py:   class Admin(User): pass
来源：http://vvd.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://ooj.yuanzhike.top

JS:   class Admin extends User {}
来源：http://wmp.jyoumei.cn

TS:   class Admin extends User {}
来源：http://qqx.quarkkingdee.top

Java: class Admin extends User {}
来源：http://wkh.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yta.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://nug.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://lug.iojbl.cn

[G06] 重写方法
来源：http://avf.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://cjb.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://how.sweek.top

JS:   greet() { return "admin"; }
来源：http://axf.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://ofx.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://dsi.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://amc.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://bdf.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://zpa.gaohongyu789.top

[G07] 调用父类方法
来源：http://jdd.xinyue.icu

Py:   super().greet()
来源：http://vrn.zhoulong.xyz

PHP:  parent::greet();
来源：http://eaf.sweek.top

JS:   super.greet();
来源：http://gaf.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://evc.ywan-chungtsiang.top

Java: super.greet();
来源：http://vcg.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ndt.fanxiaobao.xyz

Ruby: super
来源：http://alh.pycfn.com

C#:   base.Greet();
来源：http://akk.jinqigufen.top

[G08] 静态方法与属性
来源：http://vui.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pfq.tian-w.cn


<!-- 参考信息 -->