代发 wailian999

PHP:  implode(",", $items);
来源：http://fkp.yueranfly.top

JS:   items.join(",")
来源：http://lwk.gotoacloud.top

TS:   items.join(",")
来源：http://cww.316326.xyz

Java: String.join(",", items)
来源：http://blm.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://iuh.fengsongda.top

Ruby: items.join(",")
来源：http://qto.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://byf.zdbjq.cn

[E09] 去除所有空白字符
来源：http://cpb.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://njf.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jdf.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://vma.fktsv.cn

TS:   s.replace(/\s+/g, "")
来源：http://nhu.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://bwv.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qbm.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://myz.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pps.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://atv.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pgt.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wes.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://xcm.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://mje.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://ptu.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://htw.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qfu.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfp.gaohongyu789.top

[E11] 反转字符串
来源：http://uvt.jianghu66.top

Py:   s[::-1]
来源：http://new.feifeiyinyue.top

PHP:  strrev($s);
来源：http://zow.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://ltw.havefunace.top

TS:   [...s].reverse().join("")
来源：http://qhj.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kxm.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jsn.jyoumei.cn

Ruby: s.reverse
来源：http://pgh.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://dxb.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://rtl.jinqigufen.top

Py:   s.count("a")
来源：http://pyq.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://rbe.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://gpw.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://syb.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ywc.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://nvi.bjfxy.top

Ruby: s.count("a")
来源：http://orf.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://yub.guannengcc.top

[E13] 逐字符遍历
来源：http://jic.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://jiz.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dan.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wmh.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://snx.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://krh.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jlv.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jwe.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eqw.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://gij.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cpr.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fom.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jro.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wwl.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cwc.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jxu.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pgi.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ekp.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://mqh.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yae.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ihv.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hme.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rpb.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mll.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://npo.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rhh.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://evh.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://fot.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://tya.tarul.cn

PHP:  number_format(1234567);
来源：http://mfa.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ojk.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tkl.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bxb.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jdy.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://run.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://zav.cdnleiting.top

[E17] 首字母大写
来源：http://eva.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yge.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ipz.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://egs.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ymy.aizwys.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qnr.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kxg.hongshengwenyu.top

Ruby: s.capitalize
来源：http://eqf.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://byk.snrcjt.cn

[E18] 模板占位符替换
来源：http://nxs.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wgk.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yit.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ojf.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cnc.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vpj.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xwn.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://elo.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qfe.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://sio.52xcode.cn

Py:   s.splitlines()
来源：http://gbh.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwp.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://kkn.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://bbm.xuetiantiany.cn

Java: s.lines().toList()
来源：http://xwg.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://lct.fengsongda.top

Ruby: s.lines
来源：http://wtn.quarkkingdee.top

C#:   s.Split('\n')
来源：http://yld.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://nkd.bbcook.cn

Py:   if not s:
来源：http://lph.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bbp.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gdj.yj20258888.top

TS:   if (s === "") {}
来源：http://cis.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://wpn.52xcode.cn

Go:   if s == "" {}
来源：http://ybl.yvedp.cn

Ruby: if s.empty?
来源：http://nlc.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fsd.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://uld.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xwi.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vet.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fnu.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tft.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dna.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://zyi.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wsr.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cpm.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://rft.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xid.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blb.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://emg.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wqo.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://itv.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fqo.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://nkj.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wxl.jianghu66.top

================================================================================
来源：http://mbk.jlsjyb.cn

F. 文件与目录
来源：http://xga.hesvh.cn

================================================================================
来源：http://yoj.vqdsnc.cn

[F01] 读取整个文件
来源：http://hng.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hee.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://yio.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vzi.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dvm.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vml.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xso.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://clb.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://uwu.iojbl.cn

[F02] 逐行读取文件
来源：http://zcx.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mxt.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ira.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gci.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bws.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lyc.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zfy.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://exi.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nfg.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://zkk.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ekk.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nyp.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://web.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhd.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://joa.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://htk.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://jop.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://esa.fktsv.cn

[F04] 追加写入文件
来源：http://kyi.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://omi.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://phh.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avw.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tlx.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cix.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://got.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gto.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ezb.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://jwo.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aty.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://jza.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://khp.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://zkz.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bgw.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vlm.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://nve.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://psp.zdqjudy.top

[F06] 删除文件
来源：http://pme.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://pzk.cashguo.top

PHP:  unlink("a.txt");
来源：http://tmo.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iiz.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://qfy.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://smy.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://its.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://vnu.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://bvx.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://ram.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ozt.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zju.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://czb.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwa.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qyf.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vsx.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vsq.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rvc.cqqwz.cn

[F08] 遍历目录
来源：http://uhz.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://smi.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bkh.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://xvb.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://vko.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ufy.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://kay.xinyue.icu

Ruby: Dir.children("dir")
来源：http://njn.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://zxk.iojbl.cn

[F09] 获取文件大小
来源：http://xal.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://ylt.yfazqb.com

PHP:  filesize("a.txt");
来源：http://rnd.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://hru.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://nxz.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://bzb.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wma.yueranfly.top

Ruby: File.size("a.txt")
来源：http://ldt.jiagoushi.top

C#:   new FileInfo("a.txt").Length
来源：http://xsm.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ekc.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://une.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gfg.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vll.epnwcf.com

TS:   path.extname("a.txt")
来源：http://ypi.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://edy.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cxw.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ppv.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hbh.zhijiandao.cn

[F11] 复制与移动文件
来源：http://bda.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rlq.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ofw.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yry.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyd.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nop.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lca.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eix.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ltd.quarkkingdee.top

[F12] CSV 读写
来源：http://viv.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gle.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ycz.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dks.gaohongyu789.top

TS:   // 同上
来源：http://kcg.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vum.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vkm.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xcg.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pol.hnqzz.top

================================================================================
来源：http://lst.gaohongyu789.top

G. 面向对象
来源：http://pcf.ydjk.org.cn

================================================================================
来源：http://flf.cheryme.top

[G01] 定义类
来源：http://hjp.0kj1m.cn

Py:   class User: pass
来源：http://akz.andypj.xyz

PHP:  class User {}
来源：http://ifa.nanxuanxn.top

JS:   class User {}
来源：http://ejh.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://zhg.cheryme.top

Java: class User {}
来源：http://qur.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://efi.wangdashe.top

Ruby: class User; end
来源：http://vzz.wangshuangyany.cn

C#:   class User {}
来源：http://num.zhoulong.xyz

[G02] 构造函数
来源：http://ser.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://vhi.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://fzb.xinyue.icu

JS:   constructor(name) { this.name = name; }
来源：http://tgd.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://rer.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://wwh.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bmg.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://ldt.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://kiz.yongpay.top

[G03] 实例属性
来源：http://cqj.cdnleiting.top

Py:   self.name = "x"
来源：http://hnr.cqqwz.cn

PHP:  public string $name = "x";
来源：http://myg.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://uee.hnqzz.top

TS:   name: string = "x";
来源：http://naw.wangshuangyany.cn

Java: private String name;
来源：http://fym.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eyt.zdqjudy.top

Ruby: @name = "x"
来源：http://uhu.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://iyb.cashguo.top

[G04] 定义方法
来源：http://bsb.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://tqv.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tsj.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://ohr.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://nip.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://riv.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yty.zycfv.cn

Ruby: def greet; @name; end
来源：http://jan.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://lmh.gotoacloud.top

[G05] 继承
来源：http://qck.yj20258888.top

Py:   class Admin(User): pass
来源：http://okr.guannengcc.top

PHP:  class Admin extends User {}
来源：http://jrh.hywenlv.cn

JS:   class Admin extends User {}
来源：http://vju.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://vrw.tian-w.cn

Java: class Admin extends User {}
来源：http://khd.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xoj.sysykeji.top

Ruby: class Admin < User; end
来源：http://apa.ehwqpu.com

C#:   class Admin : User {}
来源：http://ltd.sweek.top

[G06] 重写方法
来源：http://kgd.yj202588.top

Py:   def greet(self): return "admin"
来源：http://ckr.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://nuk.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://irs.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://dxz.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://osf.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mid.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://dhj.feifeiyinyue.top


<!-- 参考信息 -->