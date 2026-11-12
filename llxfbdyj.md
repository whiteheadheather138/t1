代发 wailian999

PHP:  implode(",", $items);
来源：http://fmw.andypj.xyz

JS:   items.join(",")
来源：http://znv.chenlongwang.top

TS:   items.join(",")
来源：http://bpj.nwbrower.top

Java: String.join(",", items)
来源：http://qkk.meibo888.top

Go:   strings.Join(items, ",")
来源：http://vkq.gogol.net.cn

Ruby: items.join(",")
来源：http://qqy.nwbrower.top

C#:   string.Join(",", items)
来源：http://zhr.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://ilg.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hay.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eio.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://csj.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://sxd.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://thv.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yee.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://eti.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uzs.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://msd.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://acg.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://efd.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://uud.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://lzd.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://acn.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://koq.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cqh.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wbj.gaohongyu789.top

[E11] 反转字符串
来源：http://rnu.birdmap.top

Py:   s[::-1]
来源：http://pzj.havefunace.top

PHP:  strrev($s);
来源：http://ffh.tarul.cn

JS:   [...s].reverse().join("")
来源：http://fwa.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://lyo.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://okd.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bhs.fehbvm.com

Ruby: s.reverse
来源：http://zsd.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mqd.c1oappe.top

[E12] 统计某字符出现次数
来源：http://yqk.xuetiantiany.cn

Py:   s.count("a")
来源：http://kgs.uphjek.com

PHP:  substr_count($s, "a");
来源：http://aiz.aizwys.cn

JS:   s.split("a").length - 1
来源：http://rbl.yueranfly.top

TS:   s.split("a").length - 1
来源：http://pph.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iif.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://xow.fehbvm.com

Ruby: s.count("a")
来源：http://ola.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://blj.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://yip.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://kon.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://inr.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ozb.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://cws.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xvi.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pgg.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xme.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uxx.xylfe.cn

[E14] URL 编码与 Base64
来源：http://bwg.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qto.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://pxx.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://far.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ikf.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yke.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fyy.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gwo.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pxo.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://wfe.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://erh.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kjh.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://izs.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yxp.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mdn.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oil.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://psw.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mbj.meibo888.top

[E16] 数字千分位
来源：http://nlu.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://wbw.hywenlv.cn

PHP:  number_format(1234567);
来源：http://xsh.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dpx.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vad.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jku.cashguo.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nft.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnh.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://gtr.cheryme.top

[E17] 首字母大写
来源：http://jzq.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xgn.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nza.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hae.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cnl.aizwys.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aib.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qjn.daria6918.cn

Ruby: s.capitalize
来源：http://eda.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vju.havefunace.top

[E18] 模板占位符替换
来源：http://buj.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eou.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jmj.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rjr.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pso.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zzk.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://irz.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uhc.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ygx.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://svd.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://euf.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ihg.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://zrl.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://dah.gaohongyu789.top

Java: s.lines().toList()
来源：http://umh.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://ynh.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://ouj.nanxuanxn.top

C#:   s.Split('\n')
来源：http://bwn.sxryk.cn

[E20] 判断字符串是否为空
来源：http://vsi.yfazqb.com

Py:   if not s:
来源：http://nuj.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qii.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dfv.xziqi.cn

TS:   if (s === "") {}
来源：http://msb.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://bbg.jlsjyb.cn

Go:   if s == "" {}
来源：http://zli.yfazqb.com

Ruby: if s.empty?
来源：http://ozn.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lco.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://ewr.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vob.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bdo.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvd.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvc.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://avm.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://vko.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fqc.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lbk.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://wgo.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rfv.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olr.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pme.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qhq.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wvq.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cmq.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://cvw.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xkw.epnwcf.com

================================================================================
来源：http://zje.fehbvm.com

F. 文件与目录
来源：http://avj.tarul.cn

================================================================================
来源：http://ves.ppjwa.cn

[F01] 读取整个文件
来源：http://fkz.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oqu.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://yvt.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dqi.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lgg.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hun.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dhb.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://gmn.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://cxt.yangfankeji.com

[F02] 逐行读取文件
来源：http://ugp.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mgu.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fbj.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://thi.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fow.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qei.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://swj.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hbo.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qhi.yonumen.top

[F03] 写入文件（覆盖）
来源：http://nce.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cgy.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uom.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://itg.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aih.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hjr.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://afg.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://cjm.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qbv.dashuyun.cn

[F04] 追加写入文件
来源：http://npq.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wtk.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jsr.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fbc.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://foj.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fhu.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://egc.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tie.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dqk.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://sib.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://beo.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://aed.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://cnc.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://vcu.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ezv.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jhv.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://oxi.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://ynu.shanyushiyangkeji.top

[F06] 删除文件
来源：http://ska.guannengcc.top

Py:   os.remove("a.txt")
来源：http://qpm.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://ixb.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://idi.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://xfs.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yix.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://qrq.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://ndc.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://foy.andypj.xyz

[F07] 创建目录（含多级）
来源：http://puo.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpt.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://asl.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxx.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yuw.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qau.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bww.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://din.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://btv.chenzaomai.com

[F08] 遍历目录
来源：http://jut.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fnj.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ewg.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://bsw.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://soj.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bjq.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cff.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://grg.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://zrp.sjlbkw.cn

[F09] 获取文件大小
来源：http://xwg.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://kmu.yj20258888.top

PHP:  filesize("a.txt");
来源：http://vvr.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://ije.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://jxg.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ved.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dar.tian-w.cn

Ruby: File.size("a.txt")
来源：http://ylh.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://apx.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://cdj.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://szz.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjm.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kmo.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://lcp.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tni.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eja.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lff.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nff.fzhhl.top

[F11] 复制与移动文件
来源：http://zdw.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://skr.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xro.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nzu.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://orf.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pao.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gfh.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hdf.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wvx.fktsv.cn

[F12] CSV 读写
来源：http://nqy.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uig.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ssd.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://anl.vehdjk.com

TS:   // 同上
来源：http://cjt.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ahr.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jqh.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jcm.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://htk.tanke756.top

================================================================================
来源：http://foa.zhoulong.xyz

G. 面向对象
来源：http://tng.cucudq.cn

================================================================================
来源：http://jcc.yuxming.cn

[G01] 定义类
来源：http://jnb.c1oappe.top

Py:   class User: pass
来源：http://gdz.yj202588.top

PHP:  class User {}
来源：http://mvp.xinyue.icu

JS:   class User {}
来源：http://rtp.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://aju.vqdsnc.cn

Java: class User {}
来源：http://uua.jinqigufen.top

Go:   type User struct { Name string }
来源：http://hmu.jlsjyb.cn

Ruby: class User; end
来源：http://trr.yj202588.top

C#:   class User {}
来源：http://bxr.mhx1999.top

[G02] 构造函数
来源：http://ars.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://dap.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://deo.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://lao.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://paj.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://sxj.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jwk.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://qvm.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://qhj.zhengqikj.top

[G03] 实例属性
来源：http://vso.aizwys.cn

Py:   self.name = "x"
来源：http://wkb.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://ysn.zhongyouzk.top

JS:   this.name = "x";
来源：http://bwq.fktsv.cn

TS:   name: string = "x";
来源：http://wxq.zycfv.cn

Java: private String name;
来源：http://oqw.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jhg.chenlongwang.top

Ruby: @name = "x"
来源：http://uwa.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://ulz.xinyue.icu

[G04] 定义方法
来源：http://rxy.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://kbb.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ajf.havefunace.top

JS:   greet() { return this.name; }
来源：http://xov.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://kni.0kj1m.cn

Java: String greet() { return name; }
来源：http://vkn.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://nwg.cucudq.cn

Ruby: def greet; @name; end
来源：http://pmn.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://zcr.dianchejie.cn

[G05] 继承
来源：http://lmc.chenzaomai.com

Py:   class Admin(User): pass
来源：http://flm.yfazqb.com

PHP:  class Admin extends User {}
来源：http://nza.vehdjk.com

JS:   class Admin extends User {}
来源：http://wkq.sweek.top

TS:   class Admin extends User {}
来源：http://lra.gzhubu.top

Java: class Admin extends User {}
来源：http://ikz.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dua.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://mwc.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://zap.daria6918.cn

[G06] 重写方法
来源：http://ayx.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://vta.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://stq.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://mqs.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://wtj.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://vwo.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hbz.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://eie.zhoulong.xyz


<!-- 参考信息 -->