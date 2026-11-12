代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://bvw.yj20258888.top

TS:   s.split(",")
来源：http://qiu.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://ndu.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ecn.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://oat.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qzc.yueranfly.top

[E08] 数组按分隔符合并
来源：http://cev.sufxvd.cn

Py:   ",".join(items)
来源：http://mps.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://emv.chenlongwang.top

JS:   items.join(",")
来源：http://ufa.nanxuanxn.top

TS:   items.join(",")
来源：http://cvg.yfazqb.com

Java: String.join(",", items)
来源：http://dxh.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://rpq.yueranfly.top

Ruby: items.join(",")
来源：http://brz.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://xjb.hnqzz.top

[E09] 去除所有空白字符
来源：http://xmu.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ehs.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://szj.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://sbh.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://duv.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://syi.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wai.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://ygl.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iqu.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://hiu.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pmv.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ois.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://wvi.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://zqe.fehbvm.com

Java: String.format("%03d", 7)
来源：http://wsc.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zao.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uzb.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pad.wangdashe.top

[E11] 反转字符串
来源：http://hqb.redwolf501.top

Py:   s[::-1]
来源：http://vco.c1oappe.top

PHP:  strrev($s);
来源：http://grm.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://tzb.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://lzz.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://mtp.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bdm.dianchejie.cn

Ruby: s.reverse
来源：http://tgq.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lxf.tanke756.top

[E12] 统计某字符出现次数
来源：http://zlm.cdnleiting.top

Py:   s.count("a")
来源：http://hif.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://hqw.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://skm.52xcode.cn

TS:   s.split("a").length - 1
来源：http://tjl.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ztp.birdmap.top

Go:   strings.Count(s, "a")
来源：http://quf.kuanghao11.cn

Ruby: s.count("a")
来源：http://xyo.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://kcw.yanxiufei.cn

[E13] 逐字符遍历
来源：http://mby.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://stz.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jbl.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ouw.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fru.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jeq.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gja.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lqs.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pcu.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://ajq.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhz.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kyl.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uku.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gva.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ujg.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hne.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ujm.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ymw.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://sdu.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xtv.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zzs.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://msi.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ckm.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wsm.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dxw.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uph.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tgb.yj20258888.top

[E16] 数字千分位
来源：http://ymk.tarul.cn

Py:   f"{1234567:,}"
来源：http://fkl.jqgfzy.top

PHP:  number_format(1234567);
来源：http://nmd.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://faq.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://kop.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://urs.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wfs.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xqu.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://fck.sxryk.cn

[E17] 首字母大写
来源：http://qxw.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffk.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://znp.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ejs.mhx1999.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gld.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://plp.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kmx.yuxming.cn

Ruby: s.capitalize
来源：http://upf.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nes.hnxiangtu.top

[E18] 模板占位符替换
来源：http://zuz.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ksa.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://awq.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ziv.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tek.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://liw.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wxj.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gxb.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vri.zycfv.cn

[E19] 多行文本按行拆分
来源：http://ahi.hywenlv.cn

Py:   s.splitlines()
来源：http://kab.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pxy.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://oos.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://etm.svipenyu.cn

Java: s.lines().toList()
来源：http://tsd.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://ict.shuidangran.top

Ruby: s.lines
来源：http://btz.hesvh.cn

C#:   s.Split('\n')
来源：http://nep.yfazqb.com

[E20] 判断字符串是否为空
来源：http://mmd.xinyue.icu

Py:   if not s:
来源：http://rxa.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nci.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nlb.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://vtm.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://weq.daxiang520.top

Go:   if s == "" {}
来源：http://vhw.xinyue.icu

Ruby: if s.empty?
来源：http://wze.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xjf.hywenlv.cn

[E21] 超长截断加省略号
来源：http://dpu.chenlongwang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://egw.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://odr.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srm.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckf.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dzk.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://pbd.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qty.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://evz.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://oqi.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://obv.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yxl.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://luj.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fei.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nnn.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aon.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://qid.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zst.shzxlz.cn

================================================================================
来源：http://qvd.shanyushiyangkeji.top

F. 文件与目录
来源：http://gmv.chenzaomai.com

================================================================================
来源：http://qlb.chenlongwang.top

[F01] 读取整个文件
来源：http://jyf.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hno.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://jqc.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxm.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bmh.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://xfo.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rio.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://ise.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://wqo.ehwqpu.com

[F02] 逐行读取文件
来源：http://app.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eph.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tvs.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpd.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nin.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pcb.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yuk.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gse.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://owg.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://eko.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lah.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ohw.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pdj.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nex.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hzf.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ecj.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://all.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zny.hesvh.cn

[F04] 追加写入文件
来源：http://wme.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aug.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ouq.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rgr.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdd.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ywq.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vde.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nsb.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mna.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://xab.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://plz.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://psq.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://php.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://fev.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ohg.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://luk.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://ljl.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://wzm.dianchejie.cn

[F06] 删除文件
来源：http://plh.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://kuz.havefunace.top

PHP:  unlink("a.txt");
来源：http://sud.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://mfc.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://jmw.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zhf.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://ies.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://wmr.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://kot.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://aly.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dql.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gup.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uuo.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bcl.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aok.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lsz.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nyo.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zkq.bbcook.cn

[F08] 遍历目录
来源：http://xka.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lbt.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://keg.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://zik.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://lsg.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zax.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xgm.yuxming.cn

Ruby: Dir.children("dir")
来源：http://ehb.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://hwu.fktsv.cn

[F09] 获取文件大小
来源：http://hfs.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://ale.hnqzz.top

PHP:  filesize("a.txt");
来源：http://akr.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://nbs.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://kks.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ixm.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://enq.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://ntj.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://mmz.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://awc.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hje.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgg.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cvh.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://mep.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fks.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fhc.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nqb.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jpe.vqdsnc.cn

[F11] 复制与移动文件
来源：http://tgb.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qyo.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ovv.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjw.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbk.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ooy.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wmo.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zaw.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rwl.ydjk.org.cn

[F12] CSV 读写
来源：http://uer.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uzw.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pfy.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uah.gotoacloud.top

TS:   // 同上
来源：http://bvw.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mil.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgp.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zos.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bjs.ctjpmb.com

================================================================================
来源：http://ulb.uphjek.com

G. 面向对象
来源：http://ggm.aibaodan.cn

================================================================================
来源：http://tax.chenjidiqi.icu

[G01] 定义类
来源：http://oqf.jqgfzy.top

Py:   class User: pass
来源：http://hje.hcnkem.com

PHP:  class User {}
来源：http://thg.cashguo.top

JS:   class User {}
来源：http://nuo.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://ejv.fengsongda.top

Java: class User {}
来源：http://cvk.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://hfa.bjfxy.top

Ruby: class User; end
来源：http://bcf.vehdjk.com

C#:   class User {}
来源：http://lgr.nanxinkj.top

[G02] 构造函数
来源：http://ysn.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://njq.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://ybw.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://fyl.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://dmz.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://jyz.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hzc.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://uhi.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://fyn.yueranfly.top

[G03] 实例属性
来源：http://lii.vehdjk.com

Py:   self.name = "x"
来源：http://yqc.hesvh.cn

PHP:  public string $name = "x";
来源：http://pwa.bjfxy.top

JS:   this.name = "x";
来源：http://npb.jinqigfzy.top

TS:   name: string = "x";
来源：http://lno.gotoacloud.top

Java: private String name;
来源：http://itb.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qle.aibaodan.cn

Ruby: @name = "x"
来源：http://mhr.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://zpx.fzhhl.top

[G04] 定义方法
来源：http://hba.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://zid.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lnp.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://gtu.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://lwe.chenlongwang.top

Java: String greet() { return name; }
来源：http://wzj.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://bry.wangdashe.top

Ruby: def greet; @name; end
来源：http://kss.cashguo.top

C#:   public string Greet() => Name;
来源：http://zzo.smart0.xyz

[G05] 继承
来源：http://yql.zhengqikj.top

Py:   class Admin(User): pass
来源：http://tsn.ybcxt.top

PHP:  class Admin extends User {}
来源：http://yxg.aizwys.cn

JS:   class Admin extends User {}
来源：http://ivz.gzhubu.top

TS:   class Admin extends User {}
来源：http://qaw.tarul.cn

Java: class Admin extends User {}
来源：http://jwo.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ouu.hesvh.cn

Ruby: class Admin < User; end
来源：http://ppx.nanxuanxn.top

C#:   class Admin : User {}
来源：http://kyr.shzxlz.cn


<!-- 参考信息 -->