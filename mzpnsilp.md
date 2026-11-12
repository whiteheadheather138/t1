代发 wailian999

Ruby: s.split(",");  s.split
来源：http://lll.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rri.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://lbo.tarul.cn

Py:   ",".join(items)
来源：http://iby.tanke756.top

PHP:  implode(",", $items);
来源：http://qhs.xuanzx.com

JS:   items.join(",")
来源：http://ucx.tian-w.cn

TS:   items.join(",")
来源：http://dgt.smart0.xyz

Java: String.join(",", items)
来源：http://rom.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://gvp.xuetiantiany.cn

Ruby: items.join(",")
来源：http://okn.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://iel.yuanzhike.top

[E09] 去除所有空白字符
来源：http://iqg.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xkc.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qrw.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://wet.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://izt.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://byw.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://evd.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://evs.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rnk.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://zqp.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fda.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wuh.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://ciq.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://mmc.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://nvn.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://prm.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hvs.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://amb.0kj1m.cn

[E11] 反转字符串
来源：http://yor.dashuyun.cn

Py:   s[::-1]
来源：http://qgp.smart0.xyz

PHP:  strrev($s);
来源：http://upa.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://nkd.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://jpe.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bal.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://pkc.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://ozd.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xtk.yvedp.cn

[E12] 统计某字符出现次数
来源：http://hhc.jqgufenzy.top

Py:   s.count("a")
来源：http://hsx.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://qsy.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://iwe.daxiang520.top

TS:   s.split("a").length - 1
来源：http://fag.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lam.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://rne.yuxming.cn

Ruby: s.count("a")
来源：http://afs.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://lwh.vqdsnc.cn

[E13] 逐字符遍历
来源：http://jwf.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://wpf.xingfuxueyuan.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uim.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://izx.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wqn.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://krc.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gps.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mnl.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wph.zycfv.cn

[E14] URL 编码与 Base64
来源：http://gct.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tpk.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzd.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vvx.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yne.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zqv.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ekx.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nqx.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ifm.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://ayd.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://szo.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wzs.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://exs.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yap.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cec.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hza.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zlv.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lop.xuanzx.com

[E16] 数字千分位
来源：http://rht.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://jsp.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://ghv.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cxk.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://deg.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rqm.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ubw.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lmf.yongpay.top

C#:   1234567.ToString("N0")
来源：http://fmw.fehbvm.com

[E17] 首字母大写
来源：http://ucp.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tjw.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kip.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ebt.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wja.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mji.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ndl.zhaomingkeji.xyz

Ruby: s.capitalize
来源：http://guv.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yye.daxiang520.top

[E18] 模板占位符替换
来源：http://xfc.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gib.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bid.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yvc.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wvb.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kog.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nzf.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hvx.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uup.yj20258.top

[E19] 多行文本按行拆分
来源：http://mvg.tanke756.top

Py:   s.splitlines()
来源：http://nux.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jrm.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://ujj.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://ewm.nwbrower.top

Java: s.lines().toList()
来源：http://emq.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://ppu.guowangkeji.top

Ruby: s.lines
来源：http://wik.jiagoushi.top

C#:   s.Split('\n')
来源：http://pjs.52xcode.cn

[E20] 判断字符串是否为空
来源：http://kpp.sweek.top

Py:   if not s:
来源：http://kok.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wfa.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ymf.yonumen.top

TS:   if (s === "") {}
来源：http://hgu.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://www.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://ldh.shangyingyoupin.top

Ruby: if s.empty?
来源：http://hkm.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nmj.cucudq.cn

[E21] 超长截断加省略号
来源：http://hhr.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ixo.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xth.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vbl.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrk.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://apc.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://vae.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lnc.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oig.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://kop.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wkd.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nuw.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dst.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vqe.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nwa.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xxj.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://kmz.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kog.tian-w.cn

================================================================================
来源：http://zso.fzhhl.top

F. 文件与目录
来源：http://nxx.gotoacloud.top

================================================================================
来源：http://jog.chenjidiqi.icu

[F01] 读取整个文件
来源：http://yta.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dit.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://ceo.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://klt.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hpt.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ywq.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lxk.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://otr.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://snj.cdnleiting.top

[F02] 逐行读取文件
来源：http://rka.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aov.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ngu.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rox.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mdl.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wmn.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zal.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sxk.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://caj.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://qod.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ajz.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fub.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hmg.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://diy.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uoa.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vgj.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://xjk.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yql.nanxinkj.top

[F04] 追加写入文件
来源：http://ymx.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fgq.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yjf.chenzaomai.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://feg.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyt.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zhy.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rou.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nsp.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yod.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://maa.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://szd.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://jan.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://ioy.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://ezo.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zxk.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xzl.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://fco.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://nhs.zhoulong.xyz

[F06] 删除文件
来源：http://eit.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://kos.epnwcf.com

PHP:  unlink("a.txt");
来源：http://lcp.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://pfo.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://ebd.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ngw.yonumen.top

Go:   os.Remove("a.txt")
来源：http://wul.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://vac.birdmap.top

C#:   File.Delete("a.txt");
来源：http://kqj.cheryme.top

[F07] 创建目录（含多级）
来源：http://ypi.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vsz.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zsb.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vwd.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zgm.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://orm.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lcq.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://taz.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lkg.svipenyu.cn

[F08] 遍历目录
来源：http://eqq.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://eco.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kqk.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://ozy.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://xqm.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ksl.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://kzs.c1oappe.top

Ruby: Dir.children("dir")
来源：http://dwx.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://vco.hysaishi.cn

[F09] 获取文件大小
来源：http://mmc.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://cle.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://qps.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://idf.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://dnp.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ckt.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wqi.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://ewy.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://zsk.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://mxv.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cma.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pbl.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qkq.shuidangran.top

TS:   path.extname("a.txt")
来源：http://gja.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ryv.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sgx.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iir.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://noc.tanke756.top

[F11] 复制与移动文件
来源：http://rkx.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oot.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://stb.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hao.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mep.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jxb.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dlq.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jpw.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wzx.zycfv.cn

[F12] CSV 读写
来源：http://aeg.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cje.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bsa.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mfn.hongshengwenyu.top

TS:   // 同上
来源：http://srn.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iib.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qhl.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xwg.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jyl.hongshengwenyu.top

================================================================================
来源：http://rpr.jyoumei.cn

G. 面向对象
来源：http://arh.jyoumei.cn

================================================================================
来源：http://hks.havefunace.top

[G01] 定义类
来源：http://gqs.vqdsnc.cn

Py:   class User: pass
来源：http://gex.hnxiangtu.top

PHP:  class User {}
来源：http://rxv.jyoumei.cn

JS:   class User {}
来源：http://xvo.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://ymo.shangyingyoupin.top

Java: class User {}
来源：http://vsx.hammf.cn

Go:   type User struct { Name string }
来源：http://lze.ctjpmb.com

Ruby: class User; end
来源：http://jzx.redwolf501.top

C#:   class User {}
来源：http://hyj.sxryk.cn

[G02] 构造函数
来源：http://tez.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://rtd.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://bcu.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://geo.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://ajk.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://xgu.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mqn.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://huv.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://iiv.jqgufenzy.top

[G03] 实例属性
来源：http://axq.iojbl.cn

Py:   self.name = "x"
来源：http://lvx.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://xkv.fktsv.cn

JS:   this.name = "x";
来源：http://uof.fengsongda.top

TS:   name: string = "x";
来源：http://ncs.zhongyouzk.top

Java: private String name;
来源：http://gtg.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://npx.dianchejie.cn

Ruby: @name = "x"
来源：http://olf.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://ezn.jianghu66.top

[G04] 定义方法
来源：http://fll.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://oxj.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vmz.bjfxy.top

JS:   greet() { return this.name; }
来源：http://cqb.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://eng.yuxming.cn

Java: String greet() { return name; }
来源：http://usc.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ltm.hywenlv.cn

Ruby: def greet; @name; end
来源：http://nnm.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://eky.yongpay.top

[G05] 继承
来源：http://nqh.aizwys.cn

Py:   class Admin(User): pass
来源：http://xku.shuidangran.top

PHP:  class Admin extends User {}
来源：http://kyx.tanke756.top

JS:   class Admin extends User {}
来源：http://dcp.chenzaomai.com

TS:   class Admin extends User {}
来源：http://jzz.bbcook.cn

Java: class Admin extends User {}
来源：http://ixb.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://url.birdmap.top

Ruby: class Admin < User; end
来源：http://qrf.hammf.cn

C#:   class Admin : User {}
来源：http://nsm.jinghuilouyu.cn

[G06] 重写方法
来源：http://zyd.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://mol.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://keg.uphjek.com

JS:   greet() { return "admin"; }
来源：http://rml.hammf.cn


<!-- 参考信息 -->