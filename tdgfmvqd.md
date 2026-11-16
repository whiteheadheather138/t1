代发 wailian999

PHP:  implode(",", $items);
来源：http://siu.shzxlz.cn

JS:   items.join(",")
来源：http://cva.xuanzx.com

TS:   items.join(",")
来源：http://qlb.meibo888.top

Java: String.join(",", items)
来源：http://hcd.yongpay.top

Go:   strings.Join(items, ",")
来源：http://svd.sjlbkw.cn

Ruby: items.join(",")
来源：http://rsq.yuanzhike.top

C#:   string.Join(",", items)
来源：http://ufq.fzhhl.top

[E09] 去除所有空白字符
来源：http://vly.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://azc.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rsy.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://pma.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://exy.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://usk.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mvh.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wuj.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gzt.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://smc.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ehy.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ejd.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://ugp.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://hrw.guannengcc.top

Java: String.format("%03d", 7)
来源：http://jlo.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hwa.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://okn.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zag.9152youxi.cn

[E11] 反转字符串
来源：http://nym.gaohongyu789.top

Py:   s[::-1]
来源：http://sqi.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://hfk.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://nwb.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://tjy.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pqi.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nwx.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://ixv.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wih.smart0.xyz

[E12] 统计某字符出现次数
来源：http://rit.mhx1999.top

Py:   s.count("a")
来源：http://aea.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://qty.daria6918.cn

JS:   s.split("a").length - 1
来源：http://kvn.bbcook.cn

TS:   s.split("a").length - 1
来源：http://qhl.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iyf.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://nic.bjfxy.top

Ruby: s.count("a")
来源：http://gjn.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://beo.cheryme.top

[E13] 逐字符遍历
来源：http://lue.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://zpr.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bns.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wec.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nxl.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://toc.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jes.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jop.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cmc.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://omy.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qtl.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://qib.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cxb.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tok.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nyn.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zjd.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wlj.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xkn.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://ncq.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ftd.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mwt.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ujb.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tlf.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rdh.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oqg.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pxy.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wso.vehdjk.com

[E16] 数字千分位
来源：http://yjb.yongpay.top

Py:   f"{1234567:,}"
来源：http://tgc.haohaochexian.top

PHP:  number_format(1234567);
来源：http://hcm.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://igm.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ycm.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qbe.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iun.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zko.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://fgg.sufxvd.cn

[E17] 首字母大写
来源：http://rqc.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pxl.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mzl.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mjv.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iat.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yda.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oux.hammf.cn

Ruby: s.capitalize
来源：http://oqv.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hlt.fzhhl.top

[E18] 模板占位符替换
来源：http://bri.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rdk.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://stx.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nsv.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gun.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kaw.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kof.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://flg.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pld.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://jzv.xylfe.cn

Py:   s.splitlines()
来源：http://eam.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yvn.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://kfn.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://egr.zhengqikj.top

Java: s.lines().toList()
来源：http://vnx.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://dwc.bjfxy.top

Ruby: s.lines
来源：http://xmc.daxiang520.top

C#:   s.Split('\n')
来源：http://fma.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://mtf.vqdsnc.cn

Py:   if not s:
来源：http://bip.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dlh.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qoe.cashguo.top

TS:   if (s === "") {}
来源：http://ohi.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://lym.svipenyu.cn

Go:   if s == "" {}
来源：http://ajd.vehdjk.com

Ruby: if s.empty?
来源：http://pmo.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fbu.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://tst.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nya.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oed.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lre.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsv.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hid.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://klk.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://umq.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sjs.bjfxy.top

[E22] 字节长度与字符长度
来源：http://mdr.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aqc.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggh.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rmi.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fer.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ksh.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uuh.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://rju.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mnx.jinyuanbaomall.cn

================================================================================
来源：http://qrk.svipenyu.cn

F. 文件与目录
来源：http://wgf.jinqigufen.top

================================================================================
来源：http://yhg.redwolf501.top

[F01] 读取整个文件
来源：http://lav.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tzx.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://fwx.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mdh.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpt.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://gox.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uzh.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://bph.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://lai.smart0.xyz

[F02] 逐行读取文件
来源：http://tjk.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqi.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lrx.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bls.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxe.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hst.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tek.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://noe.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uqb.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://hmr.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lwt.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://klw.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpp.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sqh.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ciq.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zob.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://uet.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ioe.quarkkingdee.top

[F04] 追加写入文件
来源：http://dkw.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xpd.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cbn.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rdm.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npr.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vna.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qvu.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://liq.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ohw.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://xbd.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mjq.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://wey.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://efi.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://xaj.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cyd.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://plq.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://gxu.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://lav.ehwqpu.com

[F06] 删除文件
来源：http://qql.yongpay.top

Py:   os.remove("a.txt")
来源：http://gtv.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://ogp.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://iok.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://uzz.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ucx.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://iba.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://emo.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://ngz.sweek.top

[F07] 创建目录（含多级）
来源：http://xei.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zxy.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://naz.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xdi.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bns.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wmi.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://azc.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ymi.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nhb.ybcxt.top

[F08] 遍历目录
来源：http://cqk.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbl.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bzu.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://qll.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://lns.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cao.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://plv.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://hva.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://wdw.xylfe.cn

[F09] 获取文件大小
来源：http://qqt.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://adr.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://nge.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://nzt.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://uko.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://jjw.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dcc.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://jom.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ayi.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://tzx.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://btf.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pcm.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://unz.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://wkt.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rzx.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://txm.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zte.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://drn.guannengcc.top

[F11] 复制与移动文件
来源：http://awy.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jet.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rrn.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ujr.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://shd.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rdl.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jvl.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pnm.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://knp.zhongyouzk.top

[F12] CSV 读写
来源：http://qhg.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yie.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wcy.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yuu.daxiang520.top

TS:   // 同上
来源：http://qan.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ipp.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wkn.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nsn.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://afk.xingfuxueyuan.xyz

================================================================================
来源：http://qfj.cqqwz.cn

G. 面向对象
来源：http://hux.havefunace.top

================================================================================
来源：http://rlj.wangdashe.top

[G01] 定义类
来源：http://svw.aibaodan.cn

Py:   class User: pass
来源：http://vtc.vqdsnc.cn

PHP:  class User {}
来源：http://pog.ydjk.org.cn

JS:   class User {}
来源：http://caf.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://jsn.ppjwa.cn

Java: class User {}
来源：http://wke.cheryme.top

Go:   type User struct { Name string }
来源：http://agr.xziqi.cn

Ruby: class User; end
来源：http://jqx.cucudq.cn

C#:   class User {}
来源：http://sqo.bbcook.cn

[G02] 构造函数
来源：http://ynh.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://nes.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://rmb.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://you.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://htg.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://xvm.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rwq.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://hyh.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://ism.epnwcf.com

[G03] 实例属性
来源：http://xmc.tanke756.top

Py:   self.name = "x"
来源：http://sab.meibo888.top

PHP:  public string $name = "x";
来源：http://ksw.ppjwa.cn

JS:   this.name = "x";
来源：http://our.tian-w.cn

TS:   name: string = "x";
来源：http://wyh.shzxlz.cn

Java: private String name;
来源：http://uuy.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oos.chenjidiqi.icu

Ruby: @name = "x"
来源：http://tjh.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://vgb.hongshengwenyu.top

[G04] 定义方法
来源：http://epp.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://hkj.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dxt.fktsv.cn

JS:   greet() { return this.name; }
来源：http://cye.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://zqj.haohaochexian.top

Java: String greet() { return name; }
来源：http://gov.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jhb.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://vhe.316326.xyz

C#:   public string Greet() => Name;
来源：http://yjz.guannengcc.top

[G05] 继承
来源：http://ghc.dashuyun.cn

Py:   class Admin(User): pass
来源：http://mlq.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://eun.guannengcc.top

JS:   class Admin extends User {}
来源：http://iir.c1oappe.top

TS:   class Admin extends User {}
来源：http://zmv.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://isr.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zlt.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://dzf.aizwys.cn

C#:   class Admin : User {}
来源：http://jbw.shanyushiyangtech.top

[G06] 重写方法
来源：http://eiz.cheryme.top

Py:   def greet(self): return "admin"
来源：http://rzp.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fyl.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://orl.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://hft.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://iby.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uzi.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://fhm.yuanzhike.top


<!-- 参考信息 -->