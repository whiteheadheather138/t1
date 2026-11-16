代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xmr.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tff.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://mcm.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://gmh.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://tre.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iyy.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://crq.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cul.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://pei.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ure.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aai.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://hfi.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://qij.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://lzy.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fvs.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tia.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gdt.9152youxi.cn

[E11] 反转字符串
来源：http://qlp.fehbvm.com

Py:   s[::-1]
来源：http://tvt.hnxiangtu.top

PHP:  strrev($s);
来源：http://crc.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://qgt.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://djy.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bbb.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ufa.jiagoushi.top

Ruby: s.reverse
来源：http://djp.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://owh.fzhhl.top

[E12] 统计某字符出现次数
来源：http://mkq.chenzaomai.com

Py:   s.count("a")
来源：http://nwq.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://lvf.yfazqb.com

JS:   s.split("a").length - 1
来源：http://kjr.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://gbd.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jfj.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://pju.pycfn.com

Ruby: s.count("a")
来源：http://teu.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://nuj.tanke756.top

[E13] 逐字符遍历
来源：http://zcr.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://ujz.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mnz.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xkp.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://knp.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rbx.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cfz.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mes.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jgp.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://rii.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wou.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tkw.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yxc.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bhq.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qbr.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sin.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nul.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fsa.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://hca.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://nqu.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://faa.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wbz.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kcp.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bms.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fto.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://akd.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oxt.jiagoushi.top

[E16] 数字千分位
来源：http://afm.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://hsi.smart0.xyz

PHP:  number_format(1234567);
来源：http://gxa.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ssr.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qlx.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nqq.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xam.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://spj.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://dpo.ydjk.org.cn

[E17] 首字母大写
来源：http://ita.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jjw.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://znb.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afj.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ygo.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tgg.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://srl.zhengqikj.top

Ruby: s.capitalize
来源：http://ltn.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hvp.cdnleiting.top

[E18] 模板占位符替换
来源：http://who.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eeu.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hfg.xziqi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qex.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://odl.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pan.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uah.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ckx.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iuu.yueranfly.top

[E19] 多行文本按行拆分
来源：http://akv.nanxuanxn.top

Py:   s.splitlines()
来源：http://fkn.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fly.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://gnk.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://jvm.yueranfly.top

Java: s.lines().toList()
来源：http://mtp.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://qms.yj20258888.top

Ruby: s.lines
来源：http://nyp.nanxinkj.top

C#:   s.Split('\n')
来源：http://jwq.bbcook.cn

[E20] 判断字符串是否为空
来源：http://vlt.chenjidiqi.icu

Py:   if not s:
来源：http://dyx.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vun.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pyy.shanyushiyangtech.top

TS:   if (s === "") {}
来源：http://nka.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://ftk.yangfankeji.com

Go:   if s == "" {}
来源：http://nci.gogol.net.cn

Ruby: if s.empty?
来源：http://kdz.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bde.zdbjq.cn

[E21] 超长截断加省略号
来源：http://nuf.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://img.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tgh.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eju.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://brk.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nmt.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://oiy.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://brz.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eda.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://tpc.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zls.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kxk.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lrk.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsy.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rsj.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eyy.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://xug.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oqj.shangyingyoupin.top

================================================================================
来源：http://kbt.haohaochexian.top

F. 文件与目录
来源：http://kao.yj202588.top

================================================================================
来源：http://dsb.ivvv.top

[F01] 读取整个文件
来源：http://xjh.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jnt.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://dgv.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eos.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fcg.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://njb.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fnw.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://ero.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://ytk.ivvv.top

[F02] 逐行读取文件
来源：http://jsy.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bcw.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xoc.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kbc.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://slg.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wjq.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ywh.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://osb.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://idt.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://yqz.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cqf.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://gci.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsq.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ufo.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kzp.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fyw.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://srz.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dti.ybcxt.top

[F04] 追加写入文件
来源：http://nhu.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xgs.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zbx.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpg.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wde.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ccu.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xqn.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bwe.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mna.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://cqf.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vka.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://fuf.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://gsw.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://wag.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kjx.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lmi.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://hsn.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://ocw.jinghuilouyu.cn

[F06] 删除文件
来源：http://lga.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://mnm.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://omu.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kir.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://qkx.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vnt.yongpay.top

Go:   os.Remove("a.txt")
来源：http://ghw.ivvv.top

Ruby: File.delete("a.txt")
来源：http://naq.birdmap.top

C#:   File.Delete("a.txt");
来源：http://fwh.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://glk.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bvi.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vjr.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjq.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lyp.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kua.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jhn.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cnt.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gko.hnqzz.top

[F08] 遍历目录
来源：http://gfg.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dgo.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ncb.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://vew.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://mbe.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gqx.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ojh.tian-w.cn

Ruby: Dir.children("dir")
来源：http://fji.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://hyd.hcnkem.com

[F09] 获取文件大小
来源：http://gwy.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://kex.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://lbj.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://ebq.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://dgo.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://tye.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gou.xinyue.icu

Ruby: File.size("a.txt")
来源：http://jfn.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://pjm.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://wpl.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xvf.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qfd.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qal.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://lln.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nac.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bgo.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zet.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://scq.tarul.cn

[F11] 复制与移动文件
来源：http://ehw.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qbc.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xry.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wkd.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wyf.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mcp.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vqy.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://scx.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sqp.dianchejie.cn

[F12] CSV 读写
来源：http://jca.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wfb.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bvy.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xbj.tianlin.xyz

TS:   // 同上
来源：http://rku.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mnb.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qsp.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oaz.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iml.yueranfly.top

================================================================================
来源：http://idx.yj202588.top

G. 面向对象
来源：http://qek.xinyue.icu

================================================================================
来源：http://eqt.xinyue.icu

[G01] 定义类
来源：http://myg.xuanzx.com

Py:   class User: pass
来源：http://plz.guannengcc.top

PHP:  class User {}
来源：http://avz.zhengqikj.top

JS:   class User {}
来源：http://vdf.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://cry.xziqi.cn

Java: class User {}
来源：http://svv.redwolf501.top

Go:   type User struct { Name string }
来源：http://ila.jinyuanbaomall.cn

Ruby: class User; end
来源：http://dvm.jinqigfzy.top

C#:   class User {}
来源：http://ixb.zdqjudy.top

[G02] 构造函数
来源：http://idu.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://oor.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://kgm.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://iqt.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://sry.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://odz.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hlo.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://ijw.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://kpu.hammf.cn

[G03] 实例属性
来源：http://dea.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://eyw.hcnkem.com

PHP:  public string $name = "x";
来源：http://wgh.hnxiangtu.top

JS:   this.name = "x";
来源：http://uir.hnxiangtu.top

TS:   name: string = "x";
来源：http://dvo.chenlongwang.top

Java: private String name;
来源：http://dho.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://awl.quarkkingdee.top

Ruby: @name = "x"
来源：http://lli.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://lxb.xuanzx.com

[G04] 定义方法
来源：http://fzm.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://yfa.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yxk.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://hnb.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://wmb.shuidangran.top

Java: String greet() { return name; }
来源：http://jzr.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://sir.sxryk.cn

Ruby: def greet; @name; end
来源：http://jmy.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://mht.ppjwa.cn

[G05] 继承
来源：http://wgc.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://cym.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://cbn.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://cju.hesvh.cn

TS:   class Admin extends User {}
来源：http://xzb.nwbrower.top

Java: class Admin extends User {}
来源：http://adg.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jte.daria6918.cn

Ruby: class Admin < User; end
来源：http://tyj.epnwcf.com

C#:   class Admin : User {}
来源：http://eym.quarkkingdee.top

[G06] 重写方法
来源：http://oxu.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://ben.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://que.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://zqy.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://qbq.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://amw.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ehz.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://fzy.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://lmi.snrcjt.cn

[G07] 调用父类方法
来源：http://mkl.yanxiufei.cn

Py:   super().greet()
来源：http://yig.hnxiangtu.top

PHP:  parent::greet();
来源：http://hmo.sjlbkw.cn

JS:   super.greet();
来源：http://swx.zhaomingkeji.xyz

TS:   super.greet();
来源：http://vvz.quarkkingdee.top

Java: super.greet();
来源：http://btu.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jlw.smart0.xyz


<!-- 参考信息 -->