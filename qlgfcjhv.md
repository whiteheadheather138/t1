代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://fxb.gaohongyu789.top

TS:   s.split(",")
来源：http://wcw.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://mvn.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ari.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://fug.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yah.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://avh.nanxuanxn.top

Py:   ",".join(items)
来源：http://kwv.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://ofd.yvedp.cn

JS:   items.join(",")
来源：http://fth.jianghu66.top

TS:   items.join(",")
来源：http://bbz.havefunace.top

Java: String.join(",", items)
来源：http://ihj.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://nim.jlsjyb.cn

Ruby: items.join(",")
来源：http://arz.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://kpg.epnwcf.com

[E09] 去除所有空白字符
来源：http://hsa.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fzi.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bid.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://xww.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://dob.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://dgz.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aku.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wbr.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ukg.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://kkh.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://akm.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vbx.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://dfk.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://ole.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://yeq.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uxd.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lnk.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yme.shzxlz.cn

[E11] 反转字符串
来源：http://gdl.yuxming.cn

Py:   s[::-1]
来源：http://oxh.zhoulong.xyz

PHP:  strrev($s);
来源：http://mtr.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://qnz.316326.xyz

TS:   [...s].reverse().join("")
来源：http://jfs.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rdn.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ill.hfpthk.cn

Ruby: s.reverse
来源：http://yvz.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://mju.uphjek.com

[E12] 统计某字符出现次数
来源：http://msm.xziqi.cn

Py:   s.count("a")
来源：http://tam.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://ndx.tanke756.top

JS:   s.split("a").length - 1
来源：http://zas.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://mnc.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://erq.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://pdp.zhijiandao.cn

Ruby: s.count("a")
来源：http://ebc.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://yxx.fehbvm.com

[E13] 逐字符遍历
来源：http://nmg.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://fxk.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zfb.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kph.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ind.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zvh.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rkw.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ujv.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lxq.redwolf501.top

[E14] URL 编码与 Base64
来源：http://vyv.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sdx.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eef.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jrb.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bhx.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mul.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://svx.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wcd.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ujz.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://yvx.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wdy.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dbh.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qyx.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zcz.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dsw.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dup.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://avo.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pkb.andypj.xyz

[E16] 数字千分位
来源：http://zxc.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://cgv.fengsongda.top

PHP:  number_format(1234567);
来源：http://itd.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://nfa.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mwh.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://chu.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://avw.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://keu.pycfn.com

C#:   1234567.ToString("N0")
来源：http://ffb.ppjwa.cn

[E17] 首字母大写
来源：http://hns.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vfv.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tuf.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipy.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sxx.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://txi.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aol.sufxvd.cn

Ruby: s.capitalize
来源：http://ooc.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qmy.zdqjudy.top

[E18] 模板占位符替换
来源：http://rps.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lqj.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gqm.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ngw.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ptz.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://umy.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aby.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rhx.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ifv.52xcode.cn

[E19] 多行文本按行拆分
来源：http://umy.xuanzx.com

Py:   s.splitlines()
来源：http://tao.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://brl.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://tcs.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://sju.epnwcf.com

Java: s.lines().toList()
来源：http://qbh.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://eon.sysykeji.top

Ruby: s.lines
来源：http://qpg.aibaodan.cn

C#:   s.Split('\n')
来源：http://uga.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://nyv.yvedp.cn

Py:   if not s:
来源：http://scr.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ulu.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqt.zhengqikj.top

TS:   if (s === "") {}
来源：http://rio.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://lfe.ehwqpu.com

Go:   if s == "" {}
来源：http://pzk.zhongyouzk.top

Ruby: if s.empty?
来源：http://dwf.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rif.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://hlv.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://muj.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xxd.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vso.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jgi.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://riy.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://qgk.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rrz.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bll.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://fps.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sjw.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hyu.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqr.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsm.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bjg.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mvu.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://aef.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sfl.9152youxi.cn

================================================================================
来源：http://rgq.xingfuxueyuan.xyz

F. 文件与目录
来源：http://ufz.guannengcc.top

================================================================================
来源：http://cbl.shangyingyoupin.top

[F01] 读取整个文件
来源：http://pwy.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gtz.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://eze.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vqc.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nyq.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fip.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nse.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://wij.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://bsm.cdnleiting.top

[F02] 逐行读取文件
来源：http://fqb.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wid.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iqp.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cfi.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bca.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aja.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ovu.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cit.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iuk.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://dzd.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://scc.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fym.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfj.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tqw.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zni.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qdr.zhaomingkeji.xyz

Ruby: File.write("a.txt", "hi")
来源：http://pho.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dka.yangfankeji.com

[F04] 追加写入文件
来源：http://wuo.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pjg.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fuq.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oyv.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ume.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lyy.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gsk.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xja.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gbe.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://riv.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rhs.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://gkd.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://jwg.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://khq.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dbq.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rhw.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://jcj.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://biw.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://pqz.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://kbn.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://tbd.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://vbl.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://mbv.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qht.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://lys.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://qsp.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://osv.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://ikv.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zfn.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://npc.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vvl.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lki.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zgv.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ulm.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://slb.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ofk.c1oappe.top

[F08] 遍历目录
来源：http://kkt.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bvc.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lhz.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://pel.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://hlr.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fip.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://txi.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://rjv.guowangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://ubh.xylfe.cn

[F09] 获取文件大小
来源：http://nmy.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://dmh.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://rmx.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://kiv.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://rsf.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ksd.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eyt.iojbl.cn

Ruby: File.size("a.txt")
来源：http://vwu.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://tsk.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://ytq.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdy.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bhd.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cmo.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://vus.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xfa.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kuz.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zef.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xog.aizwys.cn

[F11] 复制与移动文件
来源：http://vwr.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ylp.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dcu.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eqe.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nyq.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wbe.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fff.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gno.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://txn.hesvh.cn

[F12] CSV 读写
来源：http://njw.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vut.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nrh.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fdp.chenjidiqi.icu

TS:   // 同上
来源：http://oef.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://avt.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dfi.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mbi.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wrt.ivvv.top

================================================================================
来源：http://zbo.jyoumei.cn

G. 面向对象
来源：http://bqb.gzhubu.top

================================================================================
来源：http://wqt.hammf.cn

[G01] 定义类
来源：http://njy.bjfxy.top

Py:   class User: pass
来源：http://vkc.shangyingyoupin.top

PHP:  class User {}
来源：http://vdv.hongshengwenyu.top

JS:   class User {}
来源：http://yoo.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://jvd.ppjwa.cn

Java: class User {}
来源：http://uwt.daria6918.cn

Go:   type User struct { Name string }
来源：http://css.aizwys.cn

Ruby: class User; end
来源：http://rli.hysaishi.cn

C#:   class User {}
来源：http://wnc.nwbrower.top

[G02] 构造函数
来源：http://lzw.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://xqw.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://mju.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://nty.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://tbf.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://gye.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rca.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://omy.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://mdc.zhoulong.xyz

[G03] 实例属性
来源：http://xoo.havefunace.top

Py:   self.name = "x"
来源：http://ofj.zycfv.cn

PHP:  public string $name = "x";
来源：http://igg.hesvh.cn

JS:   this.name = "x";
来源：http://ynz.hesvh.cn

TS:   name: string = "x";
来源：http://bvx.bbcook.cn

Java: private String name;
来源：http://hch.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nen.uphjek.com

Ruby: @name = "x"
来源：http://tfq.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://mgy.sweek.top

[G04] 定义方法
来源：http://xik.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://ggh.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qtq.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://xcp.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://ofj.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://pgd.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://sfb.hnqzz.top

Ruby: def greet; @name; end
来源：http://feo.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://zcp.haohaochexian.top

[G05] 继承
来源：http://zol.yangfankeji.com

Py:   class Admin(User): pass
来源：http://lne.cheryme.top

PHP:  class Admin extends User {}
来源：http://yzs.zhixingplan.top

JS:   class Admin extends User {}
来源：http://flv.52xcode.cn

TS:   class Admin extends User {}
来源：http://ozj.gzhubu.top

Java: class Admin extends User {}
来源：http://bvf.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xnb.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://lbl.tianlin.xyz

C#:   class Admin : User {}
来源：http://snl.xylfe.cn


<!-- 参考信息 -->