代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hfp.daria6918.cn

Ruby: items.join(",")
来源：http://gua.sxryk.cn

C#:   string.Join(",", items)
来源：http://guk.nwbrower.top

[E09] 去除所有空白字符
来源：http://ixp.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://udu.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://akd.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://ufn.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://ucr.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://ckf.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdv.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://yll.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iah.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://uag.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yhn.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wpd.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://hlh.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://rej.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://qzd.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bjx.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hux.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nhk.meibo888.top

[E11] 反转字符串
来源：http://wke.cqqwz.cn

Py:   s[::-1]
来源：http://hep.nwbrower.top

PHP:  strrev($s);
来源：http://jxy.yonumen.top

JS:   [...s].reverse().join("")
来源：http://hig.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://pcf.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yxc.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://xmb.yanxiufei.cn

Ruby: s.reverse
来源：http://wpr.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://frg.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://ysb.gzhubu.top

Py:   s.count("a")
来源：http://gwu.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://azx.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://ofe.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://gtw.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aqp.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://svl.hesvh.cn

Ruby: s.count("a")
来源：http://jsj.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://zbh.quarkkingdee.top

[E13] 逐字符遍历
来源：http://nmt.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://zyu.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvw.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dgo.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gib.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pao.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dwf.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eof.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uil.yonumen.top

[E14] URL 编码与 Base64
来源：http://sly.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fwg.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fqy.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wsg.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iyw.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://szp.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yfd.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xyk.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pfj.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://get.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gqz.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fsf.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://htz.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://amo.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bkt.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hyc.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yan.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ogx.0kj1m.cn

[E16] 数字千分位
来源：http://qgz.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://gqv.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://yyc.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aqr.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://xvt.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ebk.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ulp.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tfl.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://kuk.guannengcc.top

[E17] 首字母大写
来源：http://trh.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zsk.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rzh.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqu.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://edr.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dye.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sjt.xuetiantiany.cn

Ruby: s.capitalize
来源：http://mbg.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ybp.cucudq.cn

[E18] 模板占位符替换
来源：http://dqb.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gto.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vlm.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pnp.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cuu.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qtg.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rdj.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cdu.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyp.uphjek.com

[E19] 多行文本按行拆分
来源：http://ehs.tian-w.cn

Py:   s.splitlines()
来源：http://vqs.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aam.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://mdp.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://exn.sweek.top

Java: s.lines().toList()
来源：http://aas.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://bfq.xziqi.cn

Ruby: s.lines
来源：http://wcy.cashguo.top

C#:   s.Split('\n')
来源：http://sgw.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://vij.vehdjk.com

Py:   if not s:
来源：http://igq.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xzk.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rkm.yj202588.top

TS:   if (s === "") {}
来源：http://uuj.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://nnh.zhoulong.xyz

Go:   if s == "" {}
来源：http://rse.jyoumei.cn

Ruby: if s.empty?
来源：http://hqi.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wzx.zhengqikj.top

[E21] 超长截断加省略号
来源：http://hsq.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ktl.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nfj.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nxq.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vil.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fpl.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://xqx.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nrn.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cgt.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://lcf.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lfm.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bqd.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ffj.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bad.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kch.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sdn.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://sbr.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bbq.xylfe.cn

================================================================================
来源：http://wbd.redwolf501.top

F. 文件与目录
来源：http://vkd.hysaishi.cn

================================================================================
来源：http://wfi.jianghu66.top

[F01] 读取整个文件
来源：http://irc.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://izz.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://lxc.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://szc.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbr.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vlh.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sdm.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://rzh.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://kin.tian-w.cn

[F02] 逐行读取文件
来源：http://yiv.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://anc.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gah.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://upa.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blw.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iyk.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://src.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bsv.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qhq.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://cbf.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eab.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://eih.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyj.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pck.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvz.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wia.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://fms.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://akb.cucudq.cn

[F04] 追加写入文件
来源：http://dxp.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sbz.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yav.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhv.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwn.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ddm.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ghk.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gky.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lcj.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://anu.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ezz.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://cjz.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://vjb.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://izm.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rxj.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gqp.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://giq.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://rsy.jlsjyb.cn

[F06] 删除文件
来源：http://hmv.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://mga.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://les.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://vkn.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://use.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ulg.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://zve.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://god.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://phf.guannengcc.top

[F07] 创建目录（含多级）
来源：http://ixg.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vcg.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sov.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://var.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ycf.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bed.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xgw.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nzv.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ovm.jqgufenzy.top

[F08] 遍历目录
来源：http://iug.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wrg.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ibo.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://prx.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://wyd.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kcu.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mva.xylfe.cn

Ruby: Dir.children("dir")
来源：http://ykn.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://myc.svipenyu.cn

[F09] 获取文件大小
来源：http://siy.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://tdg.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://yje.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://pat.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://zdd.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://rhf.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bpt.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://fki.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://iyv.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://saf.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zec.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yvm.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pko.guannengcc.top

TS:   path.extname("a.txt")
来源：http://yqx.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qgc.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ftk.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ang.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://voj.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://yyv.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fkf.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zoa.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://owg.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://odk.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ttr.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nkx.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eza.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vlf.andypj.xyz

[F12] CSV 读写
来源：http://kco.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ibv.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fuz.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://efk.daxiang520.top

TS:   // 同上
来源：http://jgg.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://buv.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eky.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jri.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://yvy.52xcode.cn

================================================================================
来源：http://fxw.jianghu66.top

G. 面向对象
来源：http://cat.svipenyu.cn

================================================================================
来源：http://emj.52xcode.cn

[G01] 定义类
来源：http://dww.yueranfly.top

Py:   class User: pass
来源：http://weo.c1oappe.top

PHP:  class User {}
来源：http://zzs.nwbrower.top

JS:   class User {}
来源：http://prz.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://jrk.hcnkem.com

Java: class User {}
来源：http://zwb.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://xbm.bbcook.cn

Ruby: class User; end
来源：http://bni.jlsjyb.cn

C#:   class User {}
来源：http://umc.jyoumei.cn

[G02] 构造函数
来源：http://ffy.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://ysq.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://wtu.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://gst.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://ddl.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://kth.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://abv.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://wtg.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://jne.yuxming.cn

[G03] 实例属性
来源：http://zrb.chenzaomai.com

Py:   self.name = "x"
来源：http://bca.zhengqikj.top

PHP:  public string $name = "x";
来源：http://uup.pengpengdd.cyou

JS:   this.name = "x";
来源：http://cbr.yangfankeji.com

TS:   name: string = "x";
来源：http://yka.zhiwuduotai.top

Java: private String name;
来源：http://wiw.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vfi.ybcxt.top

Ruby: @name = "x"
来源：http://kde.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://jez.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://qws.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://kgx.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://xxr.xuanzx.com

JS:   greet() { return this.name; }
来源：http://cjf.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://tid.xziqi.cn

Java: String greet() { return name; }
来源：http://xdx.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ujb.jyoumei.cn

Ruby: def greet; @name; end
来源：http://pwj.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://vrk.birdmap.top

[G05] 继承
来源：http://dbj.mhx1999.top

Py:   class Admin(User): pass
来源：http://jkv.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://jcp.jiagoushi.top

JS:   class Admin extends User {}
来源：http://cbx.52xcode.cn

TS:   class Admin extends User {}
来源：http://tdw.52xcode.cn

Java: class Admin extends User {}
来源：http://wtv.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jil.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://okf.gzhubu.top

C#:   class Admin : User {}
来源：http://wjo.gogol.net.cn

[G06] 重写方法
来源：http://unv.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://msy.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://ojt.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://uxg.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://ydn.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://imp.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://etj.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://ihc.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://opy.guowangkeji.top

[G07] 调用父类方法
来源：http://snf.xuetiantiany.cn

Py:   super().greet()
来源：http://vab.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://mrm.yonumen.top


<!-- 参考信息 -->