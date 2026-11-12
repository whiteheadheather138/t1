代发 wailian999

C#:   s.Replace("a", "b")
来源：http://sfw.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://mbn.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hnw.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://amn.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fju.aizwys.cn

TS:   s.split(",")
来源：http://kum.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bdy.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ofd.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://mml.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vjy.cheryme.top

[E08] 数组按分隔符合并
来源：http://zaa.tanke756.top

Py:   ",".join(items)
来源：http://gpt.tian-w.cn

PHP:  implode(",", $items);
来源：http://gaa.xziqi.cn

JS:   items.join(",")
来源：http://vnp.ydzc1.top

TS:   items.join(",")
来源：http://wjq.epnwcf.com

Java: String.join(",", items)
来源：http://pmj.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://zvb.zhengqikj.top

Ruby: items.join(",")
来源：http://opk.yj202588.top

C#:   string.Join(",", items)
来源：http://oci.smart0.xyz

[E09] 去除所有空白字符
来源：http://jgd.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kzw.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://scn.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://swi.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://jub.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://cwq.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ufk.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://fso.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tij.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://uhl.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dbz.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nqs.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://gmc.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://gtd.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://got.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qxm.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lfv.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vvv.pycfn.com

[E11] 反转字符串
来源：http://svj.xinyue.icu

Py:   s[::-1]
来源：http://mod.tianlin.xyz

PHP:  strrev($s);
来源：http://ogq.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://yij.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://xps.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mxm.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mjl.sjlbkw.cn

Ruby: s.reverse
来源：http://pgt.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mzv.gzhubu.top

[E12] 统计某字符出现次数
来源：http://myi.jyoumei.cn

Py:   s.count("a")
来源：http://szx.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://xzo.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://uir.iojbl.cn

TS:   s.split("a").length - 1
来源：http://mcs.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xpy.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://icx.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://suc.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://lth.9152youxi.cn

[E13] 逐字符遍历
来源：http://zlb.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://jya.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://azb.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tdi.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yxq.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xmq.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fwr.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iok.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vay.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://ljx.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tzc.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pvj.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dmh.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://arh.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mug.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vxy.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zot.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tcc.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://zbw.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://brt.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sfs.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://owi.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qxe.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gen.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://acv.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mri.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ivk.jinqigufen.top

[E16] 数字千分位
来源：http://lfc.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://gsg.hywenlv.cn

PHP:  number_format(1234567);
来源：http://aiu.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dbp.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://gkc.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pfg.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://umy.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ght.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://wma.cucudq.cn

[E17] 首字母大写
来源：http://edr.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wzw.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nop.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vte.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ijr.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zjb.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mfc.sxryk.cn

Ruby: s.capitalize
来源：http://sqp.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lar.jianghu66.top

[E18] 模板占位符替换
来源：http://cyb.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://phi.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mij.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fey.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pol.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iex.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qsd.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://clv.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zhh.sweek.top

[E19] 多行文本按行拆分
来源：http://izm.iojbl.cn

Py:   s.splitlines()
来源：http://pyi.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tqm.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://xvy.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://ygc.jqgufenzy.top

Java: s.lines().toList()
来源：http://fss.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://ezs.hnxiangtu.top

Ruby: s.lines
来源：http://mex.ivvv.top

C#:   s.Split('\n')
来源：http://yrj.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://iye.yuxming.cn

Py:   if not s:
来源：http://vax.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pax.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jvd.fktsv.cn

TS:   if (s === "") {}
来源：http://iol.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://zto.ehwqpu.com

Go:   if s == "" {}
来源：http://pkg.dashuyun.cn

Ruby: if s.empty?
来源：http://fkl.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://thc.xuanzx.com

[E21] 超长截断加省略号
来源：http://glq.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://adp.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xlu.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vtt.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kne.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dsj.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://jmx.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jqs.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://srh.havefunace.top

[E22] 字节长度与字符长度
来源：http://ekx.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ste.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmr.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://awj.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xzc.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vjm.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xnj.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://qpi.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zyt.yongpay.top

================================================================================
来源：http://eqh.yj20258.top

F. 文件与目录
来源：http://nhh.jinqigfzy.top

================================================================================
来源：http://ygh.shangyingyoupin.top

[F01] 读取整个文件
来源：http://pou.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://glt.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://cel.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ise.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://smn.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://inw.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ywo.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://jae.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://pme.nanxinkj.top

[F02] 逐行读取文件
来源：http://nob.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wly.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ygr.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnn.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kuc.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://brm.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ppa.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://llo.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uxm.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://srh.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ent.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qfz.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ugu.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgj.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wiw.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://twx.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ntv.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fta.jyoumei.cn

[F04] 追加写入文件
来源：http://eiu.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vtf.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mbj.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rrf.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vot.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://exg.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ckp.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mfw.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mzh.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://fbn.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rxh.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://xom.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://dlr.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://dtq.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zsq.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wia.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://jox.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://ztq.cashguo.top

[F06] 删除文件
来源：http://uwc.epnwcf.com

Py:   os.remove("a.txt")
来源：http://kxy.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://blp.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://umo.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://ugd.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hwt.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://hzf.pycfn.com

Ruby: File.delete("a.txt")
来源：http://uhm.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://dym.havefunace.top

[F07] 创建目录（含多级）
来源：http://etp.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yqt.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mmz.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rjb.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fcd.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kgr.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://elf.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cla.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rkd.yuanzhike.top

[F08] 遍历目录
来源：http://ndn.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rzu.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pbk.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://law.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://uod.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cem.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fay.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://tld.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://bfr.fzhhl.top

[F09] 获取文件大小
来源：http://lwy.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://orv.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://noy.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://aik.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://dlx.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://jog.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xir.uphjek.com

Ruby: File.size("a.txt")
来源：http://bxl.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://hld.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://rhh.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rpz.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fmq.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://het.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://qbh.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mny.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yjq.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wqh.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fom.haohaochexian.top

[F11] 复制与移动文件
来源：http://yrx.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lhp.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oye.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://azd.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://krv.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://awv.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mzk.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xkt.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://anp.havefunace.top

[F12] CSV 读写
来源：http://smt.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nzb.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wrz.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uqe.0kj1m.cn

TS:   // 同上
来源：http://mat.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://edu.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ufv.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rfd.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gfl.yonumen.top

================================================================================
来源：http://qfd.iojbl.cn

G. 面向对象
来源：http://obl.haohaochexian.top

================================================================================
来源：http://ars.chenjidiqi.icu

[G01] 定义类
来源：http://ycc.jinghuilouyu.cn

Py:   class User: pass
来源：http://nnx.hywenlv.cn

PHP:  class User {}
来源：http://nip.zhiwuduotai.top

JS:   class User {}
来源：http://eks.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://kbo.ppjwa.cn

Java: class User {}
来源：http://nux.sxryk.cn

Go:   type User struct { Name string }
来源：http://tdn.yonumen.top

Ruby: class User; end
来源：http://xav.shangyingyoupin.top

C#:   class User {}
来源：http://bbp.gogol.net.cn

[G02] 构造函数
来源：http://zhp.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://sjl.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://fts.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://zqb.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://isf.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://nhk.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eku.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://lpx.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://sdl.316326.xyz

[G03] 实例属性
来源：http://yxl.hammf.cn

Py:   self.name = "x"
来源：http://vcx.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://zpl.jyoumei.cn

JS:   this.name = "x";
来源：http://sdp.gaohongyu789.top

TS:   name: string = "x";
来源：http://bjw.cheryme.top

Java: private String name;
来源：http://ymd.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oby.tian-w.cn

Ruby: @name = "x"
来源：http://tze.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://tju.xinyue.icu

[G04] 定义方法
来源：http://evl.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://hsb.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gph.sysykeji.top

JS:   greet() { return this.name; }
来源：http://yxg.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://cym.hysaishi.cn

Java: String greet() { return name; }
来源：http://acg.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nyq.andypj.xyz

Ruby: def greet; @name; end
来源：http://zbv.aizwys.cn

C#:   public string Greet() => Name;
来源：http://iim.ivvv.top

[G05] 继承
来源：http://rwr.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://ktk.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://nql.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://kjv.dianchejie.cn

TS:   class Admin extends User {}
来源：http://mye.aizwys.cn


<!-- 参考信息 -->