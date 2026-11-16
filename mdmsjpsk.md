代发 wailian999

Ruby: s.split(",");  s.split
来源：http://mmz.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://reu.sweek.top

[E08] 数组按分隔符合并
来源：http://tgx.chenlongwang.top

Py:   ",".join(items)
来源：http://rhx.xuanzx.com

PHP:  implode(",", $items);
来源：http://nil.jinqigfzy.top

JS:   items.join(",")
来源：http://ujh.cucudq.cn

TS:   items.join(",")
来源：http://srb.tian-w.cn

Java: String.join(",", items)
来源：http://icp.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://cwx.hywenlv.cn

Ruby: items.join(",")
来源：http://lvs.hcnkem.com

C#:   string.Join(",", items)
来源：http://vuc.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://qww.sjlbkw.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xcz.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://piu.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://vjc.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://hoq.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://ikz.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nza.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yax.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uvk.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://bjv.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yjo.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dbs.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://qft.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://gmr.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://kwg.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ztx.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zks.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dam.sysykeji.top

[E11] 反转字符串
来源：http://csm.yj20258.top

Py:   s[::-1]
来源：http://jza.zhixingplan.top

PHP:  strrev($s);
来源：http://mqi.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://cwb.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://ipj.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fqv.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sqd.ppjwa.cn

Ruby: s.reverse
来源：http://dhp.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rpl.bjfxy.top

[E12] 统计某字符出现次数
来源：http://vpa.sweek.top

Py:   s.count("a")
来源：http://ert.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://btw.mhx1999.top

JS:   s.split("a").length - 1
来源：http://naq.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://acn.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fdx.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://dga.xuanzx.com

Ruby: s.count("a")
来源：http://wwp.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://cdp.sjlbkw.cn

[E13] 逐字符遍历
来源：http://xhw.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://pfv.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rgc.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aev.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lcj.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ghe.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zuo.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uop.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qfq.daxiang520.top

[E14] URL 编码与 Base64
来源：http://epx.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bow.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cae.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xzf.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tid.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aii.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://irm.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rbm.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fiu.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://eqf.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sxu.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bkz.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wwf.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wsu.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uxp.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wry.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iam.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wdz.ivvv.top

[E16] 数字千分位
来源：http://eqi.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://wke.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://wfa.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jvf.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oqt.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kzk.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jqk.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gmk.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://eoa.yanxiufei.cn

[E17] 首字母大写
来源：http://xlc.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ecc.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://guu.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fco.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tko.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eul.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rki.jianghu66.top

Ruby: s.capitalize
来源：http://rgl.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tdv.kuanghao11.cn

[E18] 模板占位符替换
来源：http://puy.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bxc.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jwh.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nre.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://onh.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tgz.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mdm.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qfw.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kly.andypj.xyz

[E19] 多行文本按行拆分
来源：http://tbj.shuidangran.top

Py:   s.splitlines()
来源：http://vyg.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vlz.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://qax.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://ekz.tanke756.top

Java: s.lines().toList()
来源：http://cqv.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://pem.jinqigfzy.top

Ruby: s.lines
来源：http://rog.ybcxt.top

C#:   s.Split('\n')
来源：http://rbf.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://isr.gotoacloud.top

Py:   if not s:
来源：http://rkh.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://weu.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sen.tanke756.top

TS:   if (s === "") {}
来源：http://ofz.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://hqi.xuetiantiany.cn

Go:   if s == "" {}
来源：http://hid.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://iji.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fcg.meibo888.top

[E21] 超长截断加省略号
来源：http://fqw.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ktc.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dei.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jrj.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lll.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pbw.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://jxc.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://atl.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oju.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://dcj.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nkk.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://psm.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rvn.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tcj.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bcl.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mzc.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://qkz.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xys.yanxiufei.cn

================================================================================
来源：http://oml.kuanghao11.cn

F. 文件与目录
来源：http://luv.guowangkeji.top

================================================================================
来源：http://gvx.yueranfly.top

[F01] 读取整个文件
来源：http://zjy.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vzh.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://vxc.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mgb.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ppj.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qzr.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nvx.tarul.cn

Ruby: File.read("a.txt")
来源：http://pam.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://gsv.sjlbkw.cn

[F02] 逐行读取文件
来源：http://nmp.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://khf.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jwv.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ohw.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uqg.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sbw.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mft.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mcq.hywenlv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://naq.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://nab.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ifv.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qpz.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://imm.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uyv.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://htf.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://myx.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://riw.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cbb.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://lxz.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ngq.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hjt.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhi.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fyl.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mfw.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lwk.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qku.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://czm.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://kxo.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pbt.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://uia.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://fsi.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://kvj.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fxq.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gpn.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://rhp.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://jmy.svipenyu.cn

[F06] 删除文件
来源：http://yuf.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://pyu.ydzc1.top

PHP:  unlink("a.txt");
来源：http://wvq.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://kdq.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aae.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mct.tanke756.top

Go:   os.Remove("a.txt")
来源：http://ttq.pycfn.com

Ruby: File.delete("a.txt")
来源：http://efw.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://dbw.cheryme.top

[F07] 创建目录（含多级）
来源：http://bje.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ixt.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oia.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehb.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://avq.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyk.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfr.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dop.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://npr.cheryme.top

[F08] 遍历目录
来源：http://frp.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://avv.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mqz.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://waf.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://umu.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iqv.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hft.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://rkp.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://ahq.haohaochexian.top

[F09] 获取文件大小
来源：http://gzj.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://ulg.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://qfy.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://bjt.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://pqj.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://vil.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ugp.shuidangran.top

Ruby: File.size("a.txt")
来源：http://rtu.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://gur.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://vzz.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://njc.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://njp.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ugh.hnqzz.top

TS:   path.extname("a.txt")
来源：http://acc.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pby.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jym.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ohi.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fry.yangfankeji.com

[F11] 复制与移动文件
来源：http://pzv.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zzi.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mbx.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qvy.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uua.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mkt.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://koa.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://smn.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aup.c1oappe.top

[F12] CSV 读写
来源：http://zvy.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ywq.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gla.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ysb.xziqi.cn

TS:   // 同上
来源：http://hhn.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gpt.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xdl.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://enp.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zuz.xylfe.cn

================================================================================
来源：http://mur.zhengqikj.top

G. 面向对象
来源：http://ial.yj20258888.top

================================================================================
来源：http://hsx.birdmap.top

[G01] 定义类
来源：http://cre.gogol.net.cn

Py:   class User: pass
来源：http://iwu.wangshuangyany.cn

PHP:  class User {}
来源：http://whr.cheryme.top

JS:   class User {}
来源：http://wax.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://xmo.shzxlz.cn

Java: class User {}
来源：http://rnt.hysaishi.cn

Go:   type User struct { Name string }
来源：http://acj.shanyushiyangkeji.top

Ruby: class User; end
来源：http://eyl.yangfankeji.com

C#:   class User {}
来源：http://wty.hesvh.cn

[G02] 构造函数
来源：http://qvc.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://bix.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://mas.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://ycc.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://mll.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://wos.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eow.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://vpr.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://mhk.shzxlz.cn

[G03] 实例属性
来源：http://imr.sufxvd.cn

Py:   self.name = "x"
来源：http://yme.gzhubu.top

PHP:  public string $name = "x";
来源：http://jir.pycfn.com

JS:   this.name = "x";
来源：http://nsl.wangdashe.top

TS:   name: string = "x";
来源：http://oev.fehbvm.com

Java: private String name;
来源：http://ieh.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bnl.cheryme.top

Ruby: @name = "x"
来源：http://jby.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://nuu.yuanzhike.top

[G04] 定义方法
来源：http://jtj.daria6918.cn

Py:   def greet(self): return self.name
来源：http://pbu.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://noh.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://hiv.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://fwp.hysaishi.cn

Java: String greet() { return name; }
来源：http://kpn.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://cea.zdqjudy.top

Ruby: def greet; @name; end
来源：http://oce.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://xvo.pengpengdd.cyou

[G05] 继承
来源：http://qkr.cheryme.top

Py:   class Admin(User): pass
来源：http://xby.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://veb.hysaishi.cn

JS:   class Admin extends User {}
来源：http://osk.zycfv.cn

TS:   class Admin extends User {}
来源：http://noz.hysaishi.cn

Java: class Admin extends User {}
来源：http://xjk.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gbb.smart0.xyz

Ruby: class Admin < User; end
来源：http://ngg.hywenlv.cn

C#:   class Admin : User {}
来源：http://kcu.ivvv.top

[G06] 重写方法
来源：http://qzk.yonumen.top

Py:   def greet(self): return "admin"
来源：http://vhr.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sxm.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://hnj.hammf.cn


<!-- 参考信息 -->