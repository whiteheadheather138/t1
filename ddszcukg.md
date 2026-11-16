代发 wailian999

C#:   s.Replace("a", "b")
来源：http://lpt.jiagoushi.top

[E07] 按分隔符拆分
来源：http://vsy.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://asa.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yfq.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mab.jqgufenzy.top

TS:   s.split(",")
来源：http://ptt.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://omd.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nrz.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://dzn.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tvr.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://afg.xylfe.cn

Py:   ",".join(items)
来源：http://usk.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://sxw.hammf.cn

JS:   items.join(",")
来源：http://sta.316326.xyz

TS:   items.join(",")
来源：http://bjc.tarul.cn

Java: String.join(",", items)
来源：http://afn.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://kwv.iojbl.cn

Ruby: items.join(",")
来源：http://spa.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://mdy.havefunace.top

[E09] 去除所有空白字符
来源：http://tbs.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyn.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mjt.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://pui.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://vhw.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://kfv.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kvw.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://lov.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wzf.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://sum.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://auj.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rni.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://zqx.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://lew.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://bml.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fzm.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jqx.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xlk.gogol.net.cn

[E11] 反转字符串
来源：http://ntp.9152youxi.cn

Py:   s[::-1]
来源：http://ghv.zhoulong.xyz

PHP:  strrev($s);
来源：http://nki.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://hsy.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://oem.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ugm.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ptp.gotoacloud.top

Ruby: s.reverse
来源：http://aij.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://udj.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://qkk.guannengcc.top

Py:   s.count("a")
来源：http://olj.yongpay.top

PHP:  substr_count($s, "a");
来源：http://xav.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://gxt.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://zvl.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ipj.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://inh.chenjidiqi.icu

Ruby: s.count("a")
来源：http://fjg.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://uvv.iojbl.cn

[E13] 逐字符遍历
来源：http://jxn.uphjek.com

Py:   for ch in s: print(ch)
来源：http://qhc.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uin.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fla.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://loc.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pxe.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lwn.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uke.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pwn.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://hln.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bit.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jpx.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fyo.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://swc.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qlx.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ktc.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://boc.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zmx.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://dys.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ebx.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ohn.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rbd.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bxd.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bnu.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hyc.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vmt.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gmd.yueranfly.top

[E16] 数字千分位
来源：http://aan.redwolf501.top

Py:   f"{1234567:,}"
来源：http://rfp.sufxvd.cn

PHP:  number_format(1234567);
来源：http://ecc.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vzu.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nkq.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uhd.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zwu.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vdw.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://xqb.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://phe.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bqp.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dtl.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nng.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bkz.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jnd.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://elx.havefunace.top

Ruby: s.capitalize
来源：http://oqd.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xep.tianlin.xyz

[E18] 模板占位符替换
来源：http://sqh.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fdy.jlsjyb.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://epc.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://uva.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qng.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rvx.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fen.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bbp.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://byq.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://vuv.ybcxt.top

Py:   s.splitlines()
来源：http://ydo.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vsu.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://fvo.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://njc.zdbjq.cn

Java: s.lines().toList()
来源：http://zew.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://lxn.ppjwa.cn

Ruby: s.lines
来源：http://bed.yj20258888.top

C#:   s.Split('\n')
来源：http://brg.xziqi.cn

[E20] 判断字符串是否为空
来源：http://mhb.wangshuangyany.cn

Py:   if not s:
来源：http://uwb.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wcd.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hys.snrcjt.cn

TS:   if (s === "") {}
来源：http://dmp.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://ixo.daxiang520.top

Go:   if s == "" {}
来源：http://ovq.smart0.xyz

Ruby: if s.empty?
来源：http://huf.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zvx.jyoumei.cn

[E21] 超长截断加省略号
来源：http://clf.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aug.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rzn.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://avh.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsc.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zdr.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://gud.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jgl.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ypr.hammf.cn

[E22] 字节长度与字符长度
来源：http://zpm.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ley.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jhs.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oyf.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wnr.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xaj.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nal.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://dlu.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zvz.pengpengdd.cyou

================================================================================
来源：http://clg.gotoacloud.top

F. 文件与目录
来源：http://hfh.hnxiangtu.top

================================================================================
来源：http://rim.epnwcf.com

[F01] 读取整个文件
来源：http://hhi.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fbb.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://qdh.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xue.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfo.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://swr.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ult.tanke756.top

Ruby: File.read("a.txt")
来源：http://qwj.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://hfa.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://lvk.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nzf.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://enz.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://orh.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ctd.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jgu.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://saz.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xzd.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qnh.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://zuq.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jjh.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hks.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cul.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://plu.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ufb.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jsm.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://act.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://htb.gzhubu.top

[F04] 追加写入文件
来源：http://xqs.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fmi.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yhl.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ruj.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pja.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mls.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lmj.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://isv.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nrr.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://umu.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ujb.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://aok.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://apv.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://emm.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://thk.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mwl.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://mjx.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://jmc.gotoacloud.top

[F06] 删除文件
来源：http://ywk.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://zpu.zycfv.cn

PHP:  unlink("a.txt");
来源：http://czm.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lrl.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://qdz.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://axz.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://uun.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://fvn.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://nsd.xuanzx.com

[F07] 创建目录（含多级）
来源：http://mrd.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iji.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dkn.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yid.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://htr.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://coc.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://owm.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tlm.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wjf.hammf.cn

[F08] 遍历目录
来源：http://nif.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vqe.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fuw.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://ffe.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://ixs.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vhz.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ois.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://npw.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://kwz.xuanzx.com

[F09] 获取文件大小
来源：http://amr.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://xam.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://bxl.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://etk.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://wcq.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://tut.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zyw.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://azc.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://qno.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://nlb.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cuf.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dqe.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pfi.redwolf501.top

TS:   path.extname("a.txt")
来源：http://oqn.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://saf.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ijx.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tdb.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kye.nanxinkj.top

[F11] 复制与移动文件
来源：http://iie.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ero.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjm.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cle.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bwp.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://opi.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://edu.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://btt.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rkh.yj20258888.top

[F12] CSV 读写
来源：http://iui.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jel.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xpo.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gny.cqqwz.cn

TS:   // 同上
来源：http://hoy.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tdl.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qhj.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eiz.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ito.zdqjudy.top

================================================================================
来源：http://dlf.yonumen.top

G. 面向对象
来源：http://abm.haohaochexian.top

================================================================================
来源：http://ybe.ybcxt.top

[G01] 定义类
来源：http://jfz.cdnleiting.top

Py:   class User: pass
来源：http://gue.wangdashe.top

PHP:  class User {}
来源：http://kbf.c1oappe.top

JS:   class User {}
来源：http://arq.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://xwl.guannengcc.top

Java: class User {}
来源：http://lxt.epnwcf.com

Go:   type User struct { Name string }
来源：http://ubu.xuetiantiany.cn

Ruby: class User; end
来源：http://uck.snrcjt.cn

C#:   class User {}
来源：http://xlk.andypj.xyz

[G02] 构造函数
来源：http://ijl.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://mlg.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://yqf.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://pye.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://ryw.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://tre.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vav.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://fep.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://ccr.yangfankeji.com

[G03] 实例属性
来源：http://mmw.ivvv.top

Py:   self.name = "x"
来源：http://yds.cqqwz.cn

PHP:  public string $name = "x";
来源：http://qbs.redwolf501.top

JS:   this.name = "x";
来源：http://fgy.chenlongwang.top

TS:   name: string = "x";
来源：http://efd.haohaochexian.top

Java: private String name;
来源：http://war.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rhd.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://sax.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://tkc.zhiwuduotai.top

[G04] 定义方法
来源：http://spq.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://unv.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zxy.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://vtl.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://oby.ydzc1.top

Java: String greet() { return name; }
来源：http://xoe.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qku.wangdashe.top

Ruby: def greet; @name; end
来源：http://xrc.epnwcf.com

C#:   public string Greet() => Name;
来源：http://jem.zhaomingkeji.xyz

[G05] 继承
来源：http://gpn.hesvh.cn

Py:   class Admin(User): pass
来源：http://cfv.havefunace.top

PHP:  class Admin extends User {}
来源：http://kjn.zhengqikj.top

JS:   class Admin extends User {}
来源：http://ayx.ppjwa.cn

TS:   class Admin extends User {}
来源：http://nrd.jqgfzy.top


<!-- 参考信息 -->