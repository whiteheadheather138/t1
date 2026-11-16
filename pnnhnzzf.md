代发 wailian999

Ruby: s.split(",");  s.split
来源：http://brj.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jan.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://zvk.yfazqb.com

Py:   ",".join(items)
来源：http://ywy.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://xdu.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://rbn.xuanzx.com

TS:   items.join(",")
来源：http://bac.svipenyu.cn

Java: String.join(",", items)
来源：http://tpj.gogol.net.cn

Go:   strings.Join(items, ",")
来源：http://cai.hongshengwenyu.top

Ruby: items.join(",")
来源：http://htf.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://wpr.tianlin.xyz

[E09] 去除所有空白字符
来源：http://jpv.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mmw.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sni.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://usp.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://vyy.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://pjb.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://npr.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ukl.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kwf.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://qql.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sow.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jmj.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://qqj.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://psy.316326.xyz

Java: String.format("%03d", 7)
来源：http://wrj.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://jsg.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://awo.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rdc.zhengqikj.top

[E11] 反转字符串
来源：http://npj.yj20258888.top

Py:   s[::-1]
来源：http://ncw.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://xld.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://ccs.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://eei.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yqz.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jeo.chenjidiqi.icu

Ruby: s.reverse
来源：http://ehc.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://new.fengsongda.top

[E12] 统计某字符出现次数
来源：http://gda.hfpthk.cn

Py:   s.count("a")
来源：http://txz.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://nho.aizwys.cn

JS:   s.split("a").length - 1
来源：http://lwx.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://ugq.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://raj.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://gzk.redwolf501.top

Ruby: s.count("a")
来源：http://xfc.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://rqd.gzhubu.top

[E13] 逐字符遍历
来源：http://ogq.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://gpb.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sdr.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hjn.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zos.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ivv.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dtc.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qgi.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rne.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://sgt.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dku.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://bsh.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hwr.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dmd.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qnp.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pgs.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oep.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ewt.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://mwk.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fnj.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oce.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://inb.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qma.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ukj.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jxy.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hme.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jhh.yongpay.top

[E16] 数字千分位
来源：http://znl.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://jsp.sxryk.cn

PHP:  number_format(1234567);
来源：http://dgq.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vpr.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ihl.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lie.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dlw.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qop.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://olx.tianlin.xyz

[E17] 首字母大写
来源：http://apt.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tzc.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bwl.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xtk.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://alh.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zvl.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ejv.sjlbkw.cn

Ruby: s.capitalize
来源：http://haf.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://swp.jqgfzy.top

[E18] 模板占位符替换
来源：http://xot.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://koo.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://asn.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://faf.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xik.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ner.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jlf.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lkf.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lbr.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://tfv.shanyushiyangtech.top

Py:   s.splitlines()
来源：http://yzc.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zep.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://mco.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://swm.xinyue.icu

Java: s.lines().toList()
来源：http://deo.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://jip.0kj1m.cn

Ruby: s.lines
来源：http://zkc.0kj1m.cn

C#:   s.Split('\n')
来源：http://zru.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://mjb.ydjk.org.cn

Py:   if not s:
来源：http://lpe.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kim.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dbu.yj20258.top

TS:   if (s === "") {}
来源：http://oiu.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://wms.ybcxt.top

Go:   if s == "" {}
来源：http://wbw.hysaishi.cn

Ruby: if s.empty?
来源：http://ifw.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cai.aibaodan.cn

[E21] 超长截断加省略号
来源：http://xaq.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bbv.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gup.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mjn.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdg.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://and.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fje.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xiw.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cbw.uphjek.com

[E22] 字节长度与字符长度
来源：http://dhx.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gyf.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqv.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://odg.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ary.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nex.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gtz.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://kwz.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aqr.svipenyu.cn

================================================================================
来源：http://aou.epnwcf.com

F. 文件与目录
来源：http://dbv.jiagoushi.top

================================================================================
来源：http://cae.pycfn.com

[F01] 读取整个文件
来源：http://mef.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rsl.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://jhw.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wou.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zbp.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vkr.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://grs.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://qaz.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gyq.sysykeji.top

[F02] 逐行读取文件
来源：http://yfj.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vrx.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://meq.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ysg.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wng.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jow.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qdj.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yxv.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xhx.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://tir.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pgn.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kaj.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tfd.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uoe.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dqn.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://izg.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://lzk.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qzw.zhongyouzk.top

[F04] 追加写入文件
来源：http://kbd.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ecv.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fkv.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjt.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tlo.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uid.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pod.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lvd.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xno.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://jdi.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hgu.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://krl.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://jui.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://jnj.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xiy.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fsl.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://qli.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://ffb.nwbrower.top

[F06] 删除文件
来源：http://dkb.yongpay.top

Py:   os.remove("a.txt")
来源：http://mmp.yvedp.cn

PHP:  unlink("a.txt");
来源：http://fuq.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://vls.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://iun.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hox.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://cva.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://vxb.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://zhf.sysykeji.top

[F07] 创建目录（含多级）
来源：http://vht.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://czl.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jwo.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bkr.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://noz.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ead.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xly.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gjk.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sfn.jqgufenzy.top

[F08] 遍历目录
来源：http://oqp.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xks.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kqd.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://het.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://wko.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wsi.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vtb.yvedp.cn

Ruby: Dir.children("dir")
来源：http://fme.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://egn.guowangkeji.top

[F09] 获取文件大小
来源：http://ktx.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://fmg.smart0.xyz

PHP:  filesize("a.txt");
来源：http://zxu.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://kub.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://kjn.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://tqr.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dbe.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://qco.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://lrx.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://npt.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iha.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jvk.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kjy.nwbrower.top

TS:   path.extname("a.txt")
来源：http://iio.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mwe.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xwk.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wra.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gtz.0kj1m.cn

[F11] 复制与移动文件
来源：http://bej.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xxr.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blw.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bsi.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qsg.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zab.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iir.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oxh.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uky.yj202588.top

[F12] CSV 读写
来源：http://fyg.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tgf.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://feq.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hos.zhaomingkeji.xyz

TS:   // 同上
来源：http://hon.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mrc.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lil.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://smy.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ctj.iojbl.cn

================================================================================
来源：http://zit.gogol.net.cn

G. 面向对象
来源：http://yyw.cashguo.top

================================================================================
来源：http://tfx.yanxiufei.cn

[G01] 定义类
来源：http://vfa.chenlongwang.top

Py:   class User: pass
来源：http://qob.jqgfzy.top

PHP:  class User {}
来源：http://wka.c1oappe.top

JS:   class User {}
来源：http://lml.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://idc.jqgufenzy.top

Java: class User {}
来源：http://scq.haohaochexian.top

Go:   type User struct { Name string }
来源：http://jfh.shzxlz.cn

Ruby: class User; end
来源：http://cuy.jinqigfzy.top

C#:   class User {}
来源：http://qaf.redwolf501.top

[G02] 构造函数
来源：http://hir.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://dai.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://des.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://tge.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://iot.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://unp.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jzy.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://whg.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://yio.xinyue.icu

[G03] 实例属性
来源：http://zby.smart0.xyz

Py:   self.name = "x"
来源：http://dkk.tian-w.cn

PHP:  public string $name = "x";
来源：http://van.andypj.xyz

JS:   this.name = "x";
来源：http://wfh.gotoacloud.top

TS:   name: string = "x";
来源：http://trq.jinyuanbaomall.cn

Java: private String name;
来源：http://odp.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xeg.zhixingplan.top

Ruby: @name = "x"
来源：http://ynk.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://gga.cqqwz.cn

[G04] 定义方法
来源：http://khs.smart0.xyz

Py:   def greet(self): return self.name
来源：http://dtu.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yew.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://ayl.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://iov.zhixingplan.top

Java: String greet() { return name; }
来源：http://oih.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xpl.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://nfx.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://xoq.sjlbkw.cn

[G05] 继承
来源：http://yub.jinqigufen.top

Py:   class Admin(User): pass
来源：http://gac.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://ble.yvedp.cn

JS:   class Admin extends User {}
来源：http://yom.zycfv.cn

TS:   class Admin extends User {}
来源：http://law.fzhhl.top

Java: class Admin extends User {}
来源：http://xml.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ykv.sysykeji.top

Ruby: class Admin < User; end
来源：http://edu.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://xjh.0kj1m.cn

[G06] 重写方法
来源：http://fwm.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://yth.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nmr.yongpay.top

JS:   greet() { return "admin"; }
来源：http://xmh.sxryk.cn


<!-- 参考信息 -->