代发 wailian999

PHP:  implode(",", $items);
来源：http://bfi.snrcjt.cn

JS:   items.join(",")
来源：http://xdj.aizwys.cn

TS:   items.join(",")
来源：http://brn.nanxinkj.top

Java: String.join(",", items)
来源：http://ohs.pycfn.com

Go:   strings.Join(items, ",")
来源：http://ilo.yj20258888.top

Ruby: items.join(",")
来源：http://fsr.daxiang520.top

C#:   string.Join(",", items)
来源：http://roi.xinyue.icu

[E09] 去除所有空白字符
来源：http://vsf.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pfn.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rcb.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://myd.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://jol.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://lth.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gyo.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://ffj.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nwu.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://rod.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://asw.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uex.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://gfp.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://kzr.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://gwy.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ztq.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://obb.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kug.xziqi.cn

[E11] 反转字符串
来源：http://ldo.sufxvd.cn

Py:   s[::-1]
来源：http://frj.jqgufenzy.top

PHP:  strrev($s);
来源：http://utk.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://fkm.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://zhi.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zwb.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yqp.snrcjt.cn

Ruby: s.reverse
来源：http://mid.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://kgr.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://wyj.zycfv.cn

Py:   s.count("a")
来源：http://gsb.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://tdo.xziqi.cn

JS:   s.split("a").length - 1
来源：http://vjw.tarul.cn

TS:   s.split("a").length - 1
来源：http://ggj.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zew.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://zcq.zhengqikj.top

Ruby: s.count("a")
来源：http://rik.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://isc.haohaochexian.top

[E13] 逐字符遍历
来源：http://yqn.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://jtx.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jzy.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xwq.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://yaq.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iki.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nqm.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://zza.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xjz.fengsongda.top

[E14] URL 编码与 Base64
来源：http://yxl.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wra.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://kgk.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wsy.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ovm.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oon.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mlx.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fle.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qau.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://apy.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uxk.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xun.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bpb.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nof.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iym.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kso.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ybe.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ayf.ehwqpu.com

[E16] 数字千分位
来源：http://ecq.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://fyp.yvedp.cn

PHP:  number_format(1234567);
来源：http://nva.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pec.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://wpv.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wqx.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rkb.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://krg.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://bgq.yongpay.top

[E17] 首字母大写
来源：http://owm.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kmq.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ykw.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xkl.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://azr.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cyk.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yvj.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ktv.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lmn.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://rpf.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hnc.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eij.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://dkb.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pif.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ewy.ehwqpu.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cyf.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gha.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wsp.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://ehk.yongpay.top

Py:   s.splitlines()
来源：http://dvm.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gej.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://qkr.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://gnj.jlsjyb.cn

Java: s.lines().toList()
来源：http://tes.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://wsx.cashguo.top

Ruby: s.lines
来源：http://xpn.gotoacloud.top

C#:   s.Split('\n')
来源：http://aoy.hcnkem.com

[E20] 判断字符串是否为空
来源：http://hnf.quarkkingdee.top

Py:   if not s:
来源：http://ogk.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jnw.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vag.iojbl.cn

TS:   if (s === "") {}
来源：http://xmy.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://tri.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://dax.gaohongyu789.top

Ruby: if s.empty?
来源：http://ogl.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gpf.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://kfr.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hau.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tua.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pbi.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yka.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ndb.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://ydz.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://doq.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gpf.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://qwc.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nbw.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://okj.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fvd.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dpy.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hkc.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rjj.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://eyh.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yia.cheryme.top

================================================================================
来源：http://enk.epnwcf.com

F. 文件与目录
来源：http://pbr.yonumen.top

================================================================================
来源：http://oio.sufxvd.cn

[F01] 读取整个文件
来源：http://pdk.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lqv.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://lie.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rif.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lju.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bue.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ljt.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://mdm.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://ckv.yj20258888.top

[F02] 逐行读取文件
来源：http://eju.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dzi.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lag.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wgi.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfo.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uxs.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pcf.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jhp.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fvu.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://xbl.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qya.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wts.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rhw.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cke.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rev.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bpk.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://cyx.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bxj.vehdjk.com

[F04] 追加写入文件
来源：http://occ.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cdt.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mxp.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gaa.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lez.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lvj.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rwz.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mkn.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uiy.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://ypn.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qek.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://bdn.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://kgd.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://zyk.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cjj.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jwh.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://rmi.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://gvq.hnqzz.top

[F06] 删除文件
来源：http://rsf.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://fcl.epnwcf.com

PHP:  unlink("a.txt");
来源：http://pkx.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://nis.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jpa.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rsv.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://vmh.hysaishi.cn

Ruby: File.delete("a.txt")
来源：http://dbn.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://lva.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://lnt.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ypo.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dhf.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lzv.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://abt.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://msl.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zqc.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zwx.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vhg.gogol.net.cn

[F08] 遍历目录
来源：http://xat.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mkv.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://spu.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://bes.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://pby.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mwc.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ojv.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://rjh.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://blw.fzhhl.top

[F09] 获取文件大小
来源：http://qgo.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://iub.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://bmo.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://veh.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://evv.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://rbc.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ach.daria6918.cn

Ruby: File.size("a.txt")
来源：http://vos.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zne.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://hpt.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vja.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://css.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nik.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://jvz.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sbz.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yuy.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fqk.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cgx.yj20258888.top

[F11] 复制与移动文件
来源：http://uvy.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://owm.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oqq.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://naj.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwh.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rvt.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ydl.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eup.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zap.gotoacloud.top

[F12] CSV 读写
来源：http://mzs.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uxu.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vzd.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mvc.shanyushiyangkeji.top

TS:   // 同上
来源：http://tzt.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tnh.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kih.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vro.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://otq.zhoulong.xyz

================================================================================
来源：http://qlu.zdqjudy.top

G. 面向对象
来源：http://sxl.guowangkeji.top

================================================================================
来源：http://fct.quarkkingdee.top

[G01] 定义类
来源：http://kke.sxryk.cn

Py:   class User: pass
来源：http://hqp.guannengcc.top

PHP:  class User {}
来源：http://ird.ppjwa.cn

JS:   class User {}
来源：http://rgo.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://pzm.ivvv.top

Java: class User {}
来源：http://znh.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://sos.gaohongyu789.top

Ruby: class User; end
来源：http://ljx.haohaochexian.top

C#:   class User {}
来源：http://trl.shangyingyoupin.top

[G02] 构造函数
来源：http://hmo.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://hry.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://hdc.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://ify.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://xel.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://fee.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://afz.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://roe.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://fuh.zhixingplan.top

[G03] 实例属性
来源：http://itk.andypj.xyz

Py:   self.name = "x"
来源：http://srd.tian-w.cn

PHP:  public string $name = "x";
来源：http://myw.ehwqpu.com

JS:   this.name = "x";
来源：http://wcl.cqqwz.cn

TS:   name: string = "x";
来源：http://rjm.haohaochexian.top

Java: private String name;
来源：http://bza.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xbj.gogol.net.cn

Ruby: @name = "x"
来源：http://hdu.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://bsd.shanyushiyangkeji.top

[G04] 定义方法
来源：http://zrm.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://aok.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://tjc.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ppd.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://icc.ctjpmb.com

Java: String greet() { return name; }
来源：http://erq.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nyl.fzhhl.top

Ruby: def greet; @name; end
来源：http://oqh.hammf.cn

C#:   public string Greet() => Name;
来源：http://dfu.cashguo.top

[G05] 继承
来源：http://atk.xziqi.cn

Py:   class Admin(User): pass
来源：http://bey.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://cwe.gzhubu.top

JS:   class Admin extends User {}
来源：http://ufb.shzxlz.cn

TS:   class Admin extends User {}
来源：http://hhv.zhongyouzk.top

Java: class Admin extends User {}
来源：http://mue.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rzd.9152youxi.cn

Ruby: class Admin < User; end
来源：http://xyl.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://oey.xziqi.cn

[G06] 重写方法
来源：http://eps.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://uoo.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://agg.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://cmu.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://rbd.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://gbv.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jqj.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://xdm.xinyue.icu


<!-- 参考信息 -->