代发 wailian999

[E06] 替换子串
来源：http://tvw.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ljw.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://uit.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ipd.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://epw.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ifc.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ezc.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jwl.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://tmk.aizwys.cn

[E07] 按分隔符拆分
来源：http://ygq.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://usw.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wik.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nvl.ppjwa.cn

TS:   s.split(",")
来源：http://mqb.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fge.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zdc.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://fkf.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://urv.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://xdf.iojbl.cn

Py:   ",".join(items)
来源：http://ogd.yj202588.top

PHP:  implode(",", $items);
来源：http://fkt.hnqzz.top

JS:   items.join(",")
来源：http://zba.vqdsnc.cn

TS:   items.join(",")
来源：http://syg.xylfe.cn

Java: String.join(",", items)
来源：http://tki.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://ftj.pycfn.com

Ruby: items.join(",")
来源：http://ylq.xinyue.icu

C#:   string.Join(",", items)
来源：http://nrd.redwolf501.top

[E09] 去除所有空白字符
来源：http://llu.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jla.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jon.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://qbs.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://ket.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://wyl.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hlx.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ibr.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://abm.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://kni.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ycq.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ofc.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://jjo.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://fah.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://bqm.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uyh.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dgo.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oro.316326.xyz

[E11] 反转字符串
来源：http://wfs.jqgufenzy.top

Py:   s[::-1]
来源：http://xyk.yueranfly.top

PHP:  strrev($s);
来源：http://rky.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://iom.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://dml.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ryw.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://sok.sjlbkw.cn

Ruby: s.reverse
来源：http://iho.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://smy.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://bcf.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://hjt.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://zuj.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://ohi.sysykeji.top

TS:   s.split("a").length - 1
来源：http://cnf.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tgk.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://bxp.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://siv.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://pko.ctjpmb.com

[E13] 逐字符遍历
来源：http://lbv.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://ovt.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://arc.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qsg.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xql.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lvt.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bmz.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ftr.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zdc.pycfn.com

[E14] URL 编码与 Base64
来源：http://coq.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yzf.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://hdo.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tul.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://efj.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ddo.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wcq.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ufy.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kzw.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://hfa.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://acr.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yzp.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://srg.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://oqz.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zqb.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://suj.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nbp.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qad.mhx1999.top

[E16] 数字千分位
来源：http://djr.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://iic.zdbjq.cn

PHP:  number_format(1234567);
来源：http://ayh.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://bik.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pau.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kzi.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qsr.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://geg.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://fdu.redwolf501.top

[E17] 首字母大写
来源：http://ysi.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffj.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jct.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ctc.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kjr.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sqz.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enq.sjlbkw.cn

Ruby: s.capitalize
来源：http://aef.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iiq.wangdashe.top

[E18] 模板占位符替换
来源：http://jey.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aqs.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://myi.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yoz.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://gko.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vry.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cer.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mjr.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bxp.cashguo.top

[E19] 多行文本按行拆分
来源：http://xoj.iojbl.cn

Py:   s.splitlines()
来源：http://aoj.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vfx.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://zgj.yanxiufei.cn

TS:   s.split(/\r?\n/)
来源：http://nrr.sweek.top

Java: s.lines().toList()
来源：http://spk.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://cfk.yueranfly.top

Ruby: s.lines
来源：http://jiy.chenzaomai.com

C#:   s.Split('\n')
来源：http://fee.fengsongda.top

[E20] 判断字符串是否为空
来源：http://wtl.xinyue.icu

Py:   if not s:
来源：http://bdo.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yhq.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wrn.aibaodan.cn

TS:   if (s === "") {}
来源：http://kfc.cucudq.cn

Java: if (s.isEmpty()) {}
来源：http://rup.mhx1999.top

Go:   if s == "" {}
来源：http://hzs.xinyue.icu

Ruby: if s.empty?
来源：http://bzc.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wbc.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://rur.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ime.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fjc.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dvd.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://puz.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://key.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://avt.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cjx.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yjf.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://lbx.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ggi.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zzy.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lqt.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bfs.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sye.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vff.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://rbs.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uww.shzxlz.cn

================================================================================
来源：http://xff.guannengcc.top

F. 文件与目录
来源：http://cbg.c1oappe.top

================================================================================
来源：http://xrr.xuanzx.com

[F01] 读取整个文件
来源：http://mhc.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cee.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://ohp.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jsa.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jqw.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://bsh.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kmt.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://jlh.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gxs.sjlbkw.cn

[F02] 逐行读取文件
来源：http://iox.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uim.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rub.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcq.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zef.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vkp.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lug.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qmr.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://olq.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://vzq.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oxu.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jxa.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bee.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qlm.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nqv.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://owz.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://iux.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://its.kuanghao11.cn

[F04] 追加写入文件
来源：http://obx.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zkw.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://snl.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgc.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbt.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mbx.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xbf.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lhn.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dsy.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://bim.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mfm.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://eue.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://snq.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://wgm.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uam.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hbt.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://ten.pycfn.com

C#:   File.Exists("a.txt")
来源：http://eau.ywan-chungtsiang.top

[F06] 删除文件
来源：http://zkq.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://hcr.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://cfx.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://dih.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ont.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ffu.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://fsv.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://lbk.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://umb.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://gvw.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nsv.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://biu.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfj.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://err.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wtw.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vft.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tdq.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://djn.ydjk.org.cn

[F08] 遍历目录
来源：http://uuw.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jmx.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ptw.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://guu.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://vku.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://frm.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kti.ivvv.top

Ruby: Dir.children("dir")
来源：http://hrw.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://gvt.uphjek.com

[F09] 获取文件大小
来源：http://zqc.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ccx.wangdashe.top

PHP:  filesize("a.txt");
来源：http://eaz.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://dvj.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://tvg.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://fmo.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ifg.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://oth.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://lpu.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://iim.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wif.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://stn.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://reh.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://ixv.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://udl.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sgx.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ygp.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nub.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://ahp.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://knm.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://khb.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gmj.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpq.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://msk.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hui.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://afg.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qhf.gaohongyu789.top

[F12] CSV 读写
来源：http://cer.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://anh.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hzt.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://siv.haohaochexian.top

TS:   // 同上
来源：http://spv.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://knp.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ybu.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ohh.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://udn.0kj1m.cn

================================================================================
来源：http://zcw.jlsjyb.cn

G. 面向对象
来源：http://zru.cqqwz.cn

================================================================================
来源：http://qln.jqgufenzy.top

[G01] 定义类
来源：http://gzy.tarul.cn

Py:   class User: pass
来源：http://yal.zdqjudy.top

PHP:  class User {}
来源：http://ymy.jinqigfzy.top

JS:   class User {}
来源：http://wvc.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://bzi.sufxvd.cn

Java: class User {}
来源：http://yhj.hysaishi.cn

Go:   type User struct { Name string }
来源：http://tuz.tian-w.cn

Ruby: class User; end
来源：http://qpc.sufxvd.cn

C#:   class User {}
来源：http://tim.pengpengdd.cyou

[G02] 构造函数
来源：http://mhi.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://smy.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://twc.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://hes.sweek.top

TS:   constructor(public name: string) {}
来源：http://ccz.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://lyt.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ooq.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://cyy.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://gvv.vqdsnc.cn

[G03] 实例属性
来源：http://cju.zhiwuduotai.top

Py:   self.name = "x"
来源：http://tsh.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://ryd.sjlbkw.cn

JS:   this.name = "x";
来源：http://gdn.zdqjudy.top

TS:   name: string = "x";
来源：http://ozg.jianghu66.top

Java: private String name;
来源：http://wvi.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wlv.9152youxi.cn

Ruby: @name = "x"
来源：http://ete.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://off.jlsjyb.cn

[G04] 定义方法
来源：http://yas.jianghu66.top

Py:   def greet(self): return self.name
来源：http://sdn.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gak.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://wug.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://nup.chenzaomai.com

Java: String greet() { return name; }
来源：http://qgh.daxiang520.top


<!-- 参考信息 -->