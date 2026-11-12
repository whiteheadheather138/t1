代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://pdj.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://khs.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mmi.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iab.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://oat.yj202588.top

[E07] 按分隔符拆分
来源：http://zkv.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uml.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://axh.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sfa.aibaodan.cn

TS:   s.split(",")
来源：http://eiy.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tna.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://udt.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://xtw.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gba.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://ecl.52xcode.cn

Py:   ",".join(items)
来源：http://lfw.yvedp.cn

PHP:  implode(",", $items);
来源：http://wub.shanyushiyangtech.top

JS:   items.join(",")
来源：http://akx.shuidangran.top

TS:   items.join(",")
来源：http://itt.yonumen.top

Java: String.join(",", items)
来源：http://cck.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://tpy.yj20258888.top

Ruby: items.join(",")
来源：http://wul.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://yci.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://tmz.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ogw.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lvl.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://goc.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://vnt.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://yds.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://upf.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oaw.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zil.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://jps.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cpi.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jrf.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://vts.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://qio.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://ygf.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ijy.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rct.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nna.bbcook.cn

[E11] 反转字符串
来源：http://ykw.jqgufenzy.top

Py:   s[::-1]
来源：http://hqf.hfpthk.cn

PHP:  strrev($s);
来源：http://xie.yj202588.top

JS:   [...s].reverse().join("")
来源：http://xjw.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://jfo.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ptd.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eui.jyoumei.cn

Ruby: s.reverse
来源：http://ira.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://jjz.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://coy.yuxming.cn

Py:   s.count("a")
来源：http://ihe.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://bcx.nwbrower.top

JS:   s.split("a").length - 1
来源：http://olg.daxiang520.top

TS:   s.split("a").length - 1
来源：http://fvj.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ytk.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://nzh.zdqjudy.top

Ruby: s.count("a")
来源：http://ytn.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://pyn.sufxvd.cn

[E13] 逐字符遍历
来源：http://uwh.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://ugu.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://djy.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sac.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ulj.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nvd.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mbq.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gmg.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qrd.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://bhk.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ymk.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://qcr.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://saa.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aht.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://frd.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vzr.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://myb.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vuv.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://ugq.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://grf.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://asr.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jcp.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zil.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rvd.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zul.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pyj.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rvh.vehdjk.com

[E16] 数字千分位
来源：http://hhy.ivvv.top

Py:   f"{1234567:,}"
来源：http://jhh.yvedp.cn

PHP:  number_format(1234567);
来源：http://bwn.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mzd.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dkf.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ivx.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tzf.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cia.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://tag.ehwqpu.com

[E17] 首字母大写
来源：http://ykb.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lvk.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jbb.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xmg.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jvq.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qka.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aom.tianlin.xyz

Ruby: s.capitalize
来源：http://vua.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tee.nanxuanxn.top

[E18] 模板占位符替换
来源：http://qav.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fbe.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ebs.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zks.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fpw.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ska.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://poo.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jxq.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uha.daxiang520.top

[E19] 多行文本按行拆分
来源：http://wla.zhengqikj.top

Py:   s.splitlines()
来源：http://qrn.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eix.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://vud.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://pln.dianchejie.cn

Java: s.lines().toList()
来源：http://lsp.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://awx.fanxiaobao.xyz

Ruby: s.lines
来源：http://hxy.aizwys.cn

C#:   s.Split('\n')
来源：http://iuc.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://jxj.kuanghao11.cn

Py:   if not s:
来源：http://nkz.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ttd.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jhq.guowangkeji.top

TS:   if (s === "") {}
来源：http://mzf.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://pjg.kuanghao11.cn

Go:   if s == "" {}
来源：http://dwv.jqgufenzy.top

Ruby: if s.empty?
来源：http://ppi.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hiu.haohaochexian.top

[E21] 超长截断加省略号
来源：http://byg.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://run.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ztk.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mlv.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rbp.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wrb.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://nwr.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lrs.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bin.ybcxt.top

[E22] 字节长度与字符长度
来源：http://wam.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://far.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xwq.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bcr.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gzg.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tdo.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lof.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://tfz.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lwx.ydjk.org.cn

================================================================================
来源：http://mbd.quarkkingdee.top

F. 文件与目录
来源：http://kan.chenlongwang.top

================================================================================
来源：http://qee.aizwys.cn

[F01] 读取整个文件
来源：http://yda.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://laf.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://vpc.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pmp.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ndf.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mkw.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qmo.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://omf.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://ado.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://wpv.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xnl.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://upj.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hjk.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eoc.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lcy.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lbg.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rne.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vli.cheryme.top

[F03] 写入文件（覆盖）
来源：http://ylo.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ywj.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nxg.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kvg.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zip.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nle.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://loy.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://sye.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yhl.vqdsnc.cn

[F04] 追加写入文件
来源：http://abo.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rnw.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mak.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyv.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fto.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fga.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://glr.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fys.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fda.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://bon.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vky.yj20258.top

PHP:  file_exists("a.txt");
来源：http://soo.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://uhc.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://zgv.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vop.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mqg.sweek.top

Ruby: File.exist?("a.txt")
来源：http://gxo.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://jab.quarkkingdee.top

[F06] 删除文件
来源：http://rne.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://vkd.cucudq.cn

PHP:  unlink("a.txt");
来源：http://ief.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nld.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://ruy.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uyf.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://gza.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://inn.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://sgs.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://xvz.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vqp.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uky.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnn.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://roh.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lhi.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dqv.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xcu.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ytx.redwolf501.top

[F08] 遍历目录
来源：http://eep.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://htr.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fkn.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://lzr.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://qbh.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kvj.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fyr.hnqzz.top

Ruby: Dir.children("dir")
来源：http://pde.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://gfk.jyoumei.cn

[F09] 获取文件大小
来源：http://alc.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://blf.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://ydf.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://phq.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://lhp.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://bhr.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bvd.hesvh.cn

Ruby: File.size("a.txt")
来源：http://bti.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://iij.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://fjf.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rip.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pyc.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xih.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://zzk.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://puk.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yxp.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rzm.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://amg.havefunace.top

[F11] 复制与移动文件
来源：http://ldh.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rmp.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://byo.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nkl.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yjq.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wdx.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dpj.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jds.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bbo.pengpengdd.cyou

[F12] CSV 读写
来源：http://pbi.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hwi.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bfz.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dli.yuanzhike.top

TS:   // 同上
来源：http://hpn.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ihh.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mtm.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eyz.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lkt.jqgufenzy.top

================================================================================
来源：http://qqw.tanke756.top

G. 面向对象
来源：http://tgu.shzxlz.cn

================================================================================
来源：http://roo.ydjk.org.cn

[G01] 定义类
来源：http://mha.9152youxi.cn

Py:   class User: pass
来源：http://fqg.zhixingplan.top

PHP:  class User {}
来源：http://pwm.yj20258888.top

JS:   class User {}
来源：http://fto.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://zvg.zycfv.cn

Java: class User {}
来源：http://hof.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://pjx.jinqigufen.top

Ruby: class User; end
来源：http://wvf.andypj.xyz

C#:   class User {}
来源：http://tyw.mhx1999.top

[G02] 构造函数
来源：http://xzs.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://hvu.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://adc.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://iwt.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://zbg.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://ayj.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ukt.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://ypb.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://sud.ehwqpu.com

[G03] 实例属性
来源：http://bxr.chenzaomai.com

Py:   self.name = "x"
来源：http://ugo.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://otg.hesvh.cn

JS:   this.name = "x";
来源：http://fbh.xuetiantiany.cn

TS:   name: string = "x";
来源：http://xjd.shanyushiyangtech.top

Java: private String name;
来源：http://ayw.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ati.vehdjk.com

Ruby: @name = "x"
来源：http://uat.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://mfz.jqgfzy.top

[G04] 定义方法
来源：http://vxy.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://rks.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rjd.hammf.cn

JS:   greet() { return this.name; }
来源：http://itq.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://aze.zycfv.cn

Java: String greet() { return name; }
来源：http://mzn.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ljw.hammf.cn

Ruby: def greet; @name; end
来源：http://vga.sysykeji.top

C#:   public string Greet() => Name;
来源：http://bjt.cdnleiting.top

[G05] 继承
来源：http://jud.aibaodan.cn


<!-- 参考信息 -->