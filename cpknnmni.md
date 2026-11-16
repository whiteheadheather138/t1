代发 wailian999

Ruby: s.split(",");  s.split
来源：http://vgo.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kjq.shuidangran.top

[E08] 数组按分隔符合并
来源：http://rtz.kuanghao11.cn

Py:   ",".join(items)
来源：http://foj.iojbl.cn

PHP:  implode(",", $items);
来源：http://uez.daria6918.cn

JS:   items.join(",")
来源：http://cmg.cashguo.top

TS:   items.join(",")
来源：http://cqn.fehbvm.com

Java: String.join(",", items)
来源：http://rfd.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://tbp.ivvv.top

Ruby: items.join(",")
来源：http://qxt.ybcxt.top

C#:   string.Join(",", items)
来源：http://njg.aibaodan.cn

[E09] 去除所有空白字符
来源：http://pav.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kkm.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tdn.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://xwy.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://ttj.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://jny.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rzh.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://vxs.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://exw.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://crd.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ois.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://apt.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://peb.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://kag.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://emg.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ygt.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xbt.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vig.zhongyouzk.top

[E11] 反转字符串
来源：http://tvh.ctjpmb.com

Py:   s[::-1]
来源：http://ltx.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://sjy.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://opa.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://vdq.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gyb.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://suy.aizwys.cn

Ruby: s.reverse
来源：http://wkh.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rzd.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://dtb.yuxming.cn

Py:   s.count("a")
来源：http://moj.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://gbv.wangdashe.top

JS:   s.split("a").length - 1
来源：http://boi.cucudq.cn

TS:   s.split("a").length - 1
来源：http://guc.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dqv.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://rjt.hysaishi.cn

Ruby: s.count("a")
来源：http://nam.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://kqw.cashguo.top

[E13] 逐字符遍历
来源：http://mvl.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://epk.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fva.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnu.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://nqp.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vau.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://htj.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://srm.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jay.yj20258888.top

[E14] URL 编码与 Base64
来源：http://dvl.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pcj.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cwe.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://exx.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gkk.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wlg.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gtv.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tfa.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hei.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://ucj.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://coh.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sss.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gmp.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://oea.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qtx.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dtp.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wqw.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xey.ybcxt.top

[E16] 数字千分位
来源：http://nov.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://qlx.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://awj.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://twi.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ifv.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uva.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mnc.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vhj.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://nag.daxiang520.top

[E17] 首字母大写
来源：http://rth.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgl.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qsu.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rul.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://knx.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jqw.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eha.52xcode.cn

Ruby: s.capitalize
来源：http://kam.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yku.jyoumei.cn

[E18] 模板占位符替换
来源：http://qhs.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uto.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cob.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jyz.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zlh.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cbx.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cle.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://taz.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wug.hammf.cn

[E19] 多行文本按行拆分
来源：http://jle.yangfankeji.com

Py:   s.splitlines()
来源：http://bgj.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pkh.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://ksf.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://fzb.zhijiandao.cn

Java: s.lines().toList()
来源：http://std.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://cem.kuanghao11.cn

Ruby: s.lines
来源：http://lqf.andypj.xyz

C#:   s.Split('\n')
来源：http://vzj.vehdjk.com

[E20] 判断字符串是否为空
来源：http://ihe.yueranfly.top

Py:   if not s:
来源：http://dtr.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gtl.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sph.guowangkeji.top

TS:   if (s === "") {}
来源：http://eks.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://ptj.gotoacloud.top

Go:   if s == "" {}
来源：http://wjx.fehbvm.com

Ruby: if s.empty?
来源：http://gyi.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lkc.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://xne.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fxz.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yat.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnj.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gua.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zno.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://sjm.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zcu.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://epa.iojbl.cn

[E22] 字节长度与字符长度
来源：http://mnj.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://scw.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kfh.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mmo.hysaishi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxj.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nxl.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ajs.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://ifn.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bgp.redwolf501.top

================================================================================
来源：http://jqy.0kj1m.cn

F. 文件与目录
来源：http://iby.jianghu66.top

================================================================================
来源：http://mwe.andypj.xyz

[F01] 读取整个文件
来源：http://yvs.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jjh.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://rvp.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bkx.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jcu.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://evu.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gtl.aizwys.cn

Ruby: File.read("a.txt")
来源：http://djv.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://qzv.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://wzl.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cax.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mcg.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tbl.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxt.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://psr.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rmv.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mgl.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cwf.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://hte.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lex.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hgs.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ctm.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zvq.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://flx.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pim.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://xdl.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://unf.guannengcc.top

[F04] 追加写入文件
来源：http://vkw.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oaz.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rmu.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sie.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufc.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://enx.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ylm.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lra.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rmf.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://ftp.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pag.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://sfu.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://wrj.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://vgs.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dau.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vob.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://vhz.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://gzc.jinghuilouyu.cn

[F06] 删除文件
来源：http://zgc.fehbvm.com

Py:   os.remove("a.txt")
来源：http://dyy.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://dlp.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://tth.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://tqt.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eoz.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://sle.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://mii.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://qcv.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://oby.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ntn.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vvs.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhw.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://maf.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jvm.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zhg.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ttl.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jpk.ehwqpu.com

[F08] 遍历目录
来源：http://oqq.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qbb.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aoo.sweek.top

JS:   fs.readdirSync("dir")
来源：http://xki.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://dpd.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yca.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bkv.birdmap.top

Ruby: Dir.children("dir")
来源：http://ael.guowangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://rdn.hammf.cn

[F09] 获取文件大小
来源：http://hhg.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://aeh.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://bdk.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://nys.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://hpd.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://asi.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rhx.yfazqb.com

Ruby: File.size("a.txt")
来源：http://oyt.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://xqk.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://zuv.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fll.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eam.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wwc.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://tdl.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mod.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jji.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mqa.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gmt.nanxinkj.top

[F11] 复制与移动文件
来源：http://fwz.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cai.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gox.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ggb.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pca.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bbu.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gnq.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qjd.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eml.yj20258.top

[F12] CSV 读写
来源：http://dem.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xfk.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tzr.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lym.yueranfly.top

TS:   // 同上
来源：http://igw.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fux.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zyu.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fvn.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tzl.birdmap.top

================================================================================
来源：http://spk.zhengqikj.top

G. 面向对象
来源：http://kze.jqgfzy.top

================================================================================
来源：http://dba.cheryme.top

[G01] 定义类
来源：http://ueg.feifeiyinyue.top

Py:   class User: pass
来源：http://pdv.zhongyouzk.top

PHP:  class User {}
来源：http://lwr.jianghu66.top

JS:   class User {}
来源：http://ngc.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://ngr.hysaishi.cn

Java: class User {}
来源：http://bef.dianchejie.cn

Go:   type User struct { Name string }
来源：http://nok.snrcjt.cn

Ruby: class User; end
来源：http://xdm.fktsv.cn

C#:   class User {}
来源：http://gii.nanxinkj.top

[G02] 构造函数
来源：http://jxl.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://env.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://rst.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://wcs.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://zqr.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://inh.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tdm.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://qqp.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://xix.xuetiantiany.cn

[G03] 实例属性
来源：http://rth.316326.xyz

Py:   self.name = "x"
来源：http://voc.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://yye.zhengqikj.top

JS:   this.name = "x";
来源：http://dtj.jqgfzy.top

TS:   name: string = "x";
来源：http://cup.zhiwuduotai.top

Java: private String name;
来源：http://zpd.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ngx.gogol.net.cn

Ruby: @name = "x"
来源：http://tob.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://zii.shzxlz.cn

[G04] 定义方法
来源：http://aug.hesvh.cn

Py:   def greet(self): return self.name
来源：http://lew.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qww.sxryk.cn

JS:   greet() { return this.name; }
来源：http://ism.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://yxk.zhengqikj.top

Java: String greet() { return name; }
来源：http://quc.kuanghao11.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://azf.cqqwz.cn

Ruby: def greet; @name; end
来源：http://zws.tian-w.cn

C#:   public string Greet() => Name;
来源：http://vtp.52xcode.cn

[G05] 继承
来源：http://qzq.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://tps.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://apm.xylfe.cn

JS:   class Admin extends User {}
来源：http://yho.bjfxy.top

TS:   class Admin extends User {}
来源：http://lqe.zhixingplan.top

Java: class Admin extends User {}
来源：http://ftn.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mtb.mhx1999.top

Ruby: class Admin < User; end
来源：http://pwz.gzhubu.top

C#:   class Admin : User {}
来源：http://ogv.yuanzhike.top

[G06] 重写方法
来源：http://idp.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://krf.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://meb.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://ssu.cucudq.cn


<!-- 参考信息 -->