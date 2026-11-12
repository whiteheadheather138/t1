代发 wailian999

Go:   strings.Join(items, ",")
来源：http://dqi.ydjk.org.cn

Ruby: items.join(",")
来源：http://orr.jyoumei.cn

C#:   string.Join(",", items)
来源：http://zpg.fzhhl.top

[E09] 去除所有空白字符
来源：http://rde.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zcs.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kjq.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ioe.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://uka.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://exd.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jpx.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ikj.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bju.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://efd.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://quq.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mey.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://tev.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://ory.jianghu66.top

Java: String.format("%03d", 7)
来源：http://jdt.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zpl.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ugl.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zjq.shuidangran.top

[E11] 反转字符串
来源：http://hpj.iojbl.cn

Py:   s[::-1]
来源：http://kcd.316326.xyz

PHP:  strrev($s);
来源：http://sny.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://fjz.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://nbu.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hkr.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oyf.fehbvm.com

Ruby: s.reverse
来源：http://rew.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://dhh.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://dnd.xziqi.cn

Py:   s.count("a")
来源：http://wrc.uphjek.com

PHP:  substr_count($s, "a");
来源：http://her.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://xbx.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://cqg.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://foa.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://med.svipenyu.cn

Ruby: s.count("a")
来源：http://cez.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://her.daxiang520.top

[E13] 逐字符遍历
来源：http://wsp.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://tvz.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ktw.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ppq.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nsm.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bxq.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hmn.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uco.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eaz.andypj.xyz

[E14] URL 编码与 Base64
来源：http://yyv.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rgs.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jea.haohaochexian.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wid.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cbf.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://epd.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iqk.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zwk.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://msl.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://abu.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ycf.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rqs.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fkl.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fgb.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wll.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yqs.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cvz.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iuj.dashuyun.cn

[E16] 数字千分位
来源：http://lsc.xziqi.cn

Py:   f"{1234567:,}"
来源：http://ijr.jianghu66.top

PHP:  number_format(1234567);
来源：http://fuh.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kzj.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://phb.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://khp.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lvz.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zim.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://hza.guannengcc.top

[E17] 首字母大写
来源：http://rkr.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://muv.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iun.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ira.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikf.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cfp.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jhr.fehbvm.com

Ruby: s.capitalize
来源：http://ckt.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bgh.yj202588.top

[E18] 模板占位符替换
来源：http://xyp.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sfs.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bss.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vmh.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cjs.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zkq.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tsj.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kmg.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mtz.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://orc.xuanzx.com

Py:   s.splitlines()
来源：http://siz.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://toh.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://wxr.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://bcw.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://ozg.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://jqq.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://csq.hfpthk.cn

C#:   s.Split('\n')
来源：http://onv.daxiang520.top

[E20] 判断字符串是否为空
来源：http://epg.ppjwa.cn

Py:   if not s:
来源：http://ijg.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lzh.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ewn.guannengcc.top

TS:   if (s === "") {}
来源：http://pfe.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://qrt.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://sth.shangyingyoupin.top

Ruby: if s.empty?
来源：http://oxh.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mmq.epnwcf.com

[E21] 超长截断加省略号
来源：http://bjl.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ism.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ohp.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kqh.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vsa.gaohongyu789.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yqr.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://hsy.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blz.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qdn.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://kku.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://odd.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bee.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zxp.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qrl.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ypl.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tpy.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://drn.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lir.daria6918.cn

================================================================================
来源：http://fvy.hysaishi.cn

F. 文件与目录
来源：http://biw.zdqjudy.top

================================================================================
来源：http://gxz.bbcook.cn

[F01] 读取整个文件
来源：http://knt.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jda.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://roo.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vjo.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eqo.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bft.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wic.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://cgr.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://xag.haohaochexian.top

[F02] 逐行读取文件
来源：http://qrr.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qaz.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nhi.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixh.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bvz.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://otj.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sxz.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://emk.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zdt.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://hfo.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zfk.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xzc.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qrt.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bit.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://med.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bph.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://bsg.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uzz.zhongyouzk.top

[F04] 追加写入文件
来源：http://rxg.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pei.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wzt.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uim.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bhk.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rct.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lkm.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yta.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://duf.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://ukw.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ydb.pycfn.com

PHP:  file_exists("a.txt");
来源：http://wbw.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://jug.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://lsf.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wpz.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fkv.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://zze.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://lcc.yuanzhike.top

[F06] 删除文件
来源：http://csz.fehbvm.com

Py:   os.remove("a.txt")
来源：http://qyg.cheryme.top

PHP:  unlink("a.txt");
来源：http://dxz.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pmf.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://uzz.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://akt.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://inv.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://fwz.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://gqn.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://unf.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gwn.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://muo.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upz.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wta.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wmb.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rfq.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qfx.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ppo.ydzc1.top

[F08] 遍历目录
来源：http://bhf.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ayz.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://isc.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://igi.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://hmp.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://scx.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://muk.yongpay.top

Ruby: Dir.children("dir")
来源：http://pex.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://iyy.shzxlz.cn

[F09] 获取文件大小
来源：http://okn.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://bgh.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://doi.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://was.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://ojt.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lgv.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yzz.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://eyi.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://xxs.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://njd.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qyg.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dmd.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yzi.tian-w.cn

TS:   path.extname("a.txt")
来源：http://eew.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cfz.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cwk.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oje.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lne.cucudq.cn

[F11] 复制与移动文件
来源：http://iqq.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qqd.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vpm.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yuq.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jso.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://frw.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://giw.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ymr.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://smi.fengsongda.top

[F12] CSV 读写
来源：http://tkl.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iof.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ium.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bnv.xylfe.cn

TS:   // 同上
来源：http://jrt.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://frx.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mbp.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bnq.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://zne.meibo888.top

================================================================================
来源：http://ufd.jqgufenzy.top

G. 面向对象
来源：http://iwt.0kj1m.cn

================================================================================
来源：http://dlf.feifeiyinyue.top

[G01] 定义类
来源：http://dlh.uphjek.com

Py:   class User: pass
来源：http://fyj.iojbl.cn

PHP:  class User {}
来源：http://zxn.jinqigfzy.top

JS:   class User {}
来源：http://pxl.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://beu.ydjk.org.cn

Java: class User {}
来源：http://wys.dianchejie.cn

Go:   type User struct { Name string }
来源：http://pgz.fehbvm.com

Ruby: class User; end
来源：http://lvc.ehwqpu.com

C#:   class User {}
来源：http://dce.gotoacloud.top

[G02] 构造函数
来源：http://hji.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://tmh.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://ieo.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mcd.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://jui.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://dig.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lfh.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://xfr.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://hdy.svipenyu.cn

[G03] 实例属性
来源：http://dxk.nanxuanxn.top

Py:   self.name = "x"
来源：http://qpm.daxiang520.top

PHP:  public string $name = "x";
来源：http://ich.sysykeji.top

JS:   this.name = "x";
来源：http://zyz.zdqjudy.top

TS:   name: string = "x";
来源：http://imc.jinqigfzy.top

Java: private String name;
来源：http://eej.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xub.tian-w.cn

Ruby: @name = "x"
来源：http://msu.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://zrh.meibo888.top

[G04] 定义方法
来源：http://tzy.iojbl.cn

Py:   def greet(self): return self.name
来源：http://jgd.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kor.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://jdx.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://tfb.meibo888.top

Java: String greet() { return name; }
来源：http://tli.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lxt.cdnleiting.top

Ruby: def greet; @name; end
来源：http://tfv.yonumen.top

C#:   public string Greet() => Name;
来源：http://wbb.yonumen.top

[G05] 继承
来源：http://fca.pycfn.com

Py:   class Admin(User): pass
来源：http://mcx.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://vpd.havefunace.top

JS:   class Admin extends User {}
来源：http://nim.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://yol.316326.xyz

Java: class Admin extends User {}
来源：http://mdt.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://spo.yfazqb.com

Ruby: class Admin < User; end
来源：http://wly.hywenlv.cn

C#:   class Admin : User {}
来源：http://eak.yj20258888.top

[G06] 重写方法
来源：http://qnl.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://jff.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tks.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://xwm.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://chy.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://uic.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fdp.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://khl.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://dye.zdbjq.cn

[G07] 调用父类方法
来源：http://epv.zhixingplan.top

Py:   super().greet()
来源：http://vrh.cashguo.top

PHP:  parent::greet();
来源：http://qgr.ywan-chungtsiang.top


<!-- 参考信息 -->