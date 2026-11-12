代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uxa.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sin.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://hzj.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://enj.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://xpk.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xwq.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ugx.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://liq.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://czs.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fwq.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wtp.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://goq.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://nny.redwolf501.top

Java: String.format("%03d", 7)
来源：http://ujp.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://grm.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nsu.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iem.xziqi.cn

[E11] 反转字符串
来源：http://uqq.cdnleiting.top

Py:   s[::-1]
来源：http://yrc.guowangkeji.top

PHP:  strrev($s);
来源：http://kwj.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://jst.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://mha.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nzp.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tfv.yongpay.top

Ruby: s.reverse
来源：http://bfh.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rim.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://lgx.chenzaomai.com

Py:   s.count("a")
来源：http://bca.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://axa.cashguo.top

JS:   s.split("a").length - 1
来源：http://yaa.fktsv.cn

TS:   s.split("a").length - 1
来源：http://czi.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mrg.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://alp.gotoacloud.top

Ruby: s.count("a")
来源：http://upb.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://zhj.chenlongwang.top

[E13] 逐字符遍历
来源：http://uak.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://rwt.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fjj.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rgn.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sgn.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cxy.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xdw.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ddc.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://msj.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://ooz.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ubs.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jvp.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bgi.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vbm.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mqt.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ehz.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pnr.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zxi.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://ncf.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xkf.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ngy.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uvo.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://vhk.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://snr.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qhf.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://smn.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmk.cqqwz.cn

[E16] 数字千分位
来源：http://erj.redwolf501.top

Py:   f"{1234567:,}"
来源：http://rky.c1oappe.top

PHP:  number_format(1234567);
来源：http://jwo.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kut.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oir.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://evb.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qsu.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zeu.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://dif.yj20258888.top

[E17] 首字母大写
来源：http://ngh.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://syq.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://grf.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gkv.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kyt.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bid.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kpq.wangshuangyany.cn

Ruby: s.capitalize
来源：http://qwk.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nfw.yueranfly.top

[E18] 模板占位符替换
来源：http://hfg.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rjc.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://grl.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://igo.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jxd.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sfk.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://khq.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dis.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ial.xylfe.cn

[E19] 多行文本按行拆分
来源：http://bqv.gzhubu.top

Py:   s.splitlines()
来源：http://emq.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zmo.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://lyp.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://aik.tian-w.cn

Java: s.lines().toList()
来源：http://ndj.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://jrt.aibaodan.cn

Ruby: s.lines
来源：http://sjr.daxiang520.top

C#:   s.Split('\n')
来源：http://ngk.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://tkc.ydzc1.top

Py:   if not s:
来源：http://vfj.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pkp.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zvo.sxryk.cn

TS:   if (s === "") {}
来源：http://rzs.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://pxm.zhoulong.xyz

Go:   if s == "" {}
来源：http://xnp.yj202588.top

Ruby: if s.empty?
来源：http://guq.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hat.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://axu.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zyo.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vet.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bfr.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wrk.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://upm.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://ixi.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dhn.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mcc.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://kch.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://grx.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ise.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bto.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eyp.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fhb.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://umv.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://hfz.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://imm.0kj1m.cn

================================================================================
来源：http://gfr.bjfxy.top

F. 文件与目录
来源：http://eil.yuanzhike.top

================================================================================
来源：http://csa.snrcjt.cn

[F01] 读取整个文件
来源：http://chb.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bsk.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://kqn.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dui.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cbo.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hbf.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cgg.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://qqo.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://dbx.iojbl.cn

[F02] 逐行读取文件
来源：http://oot.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zuy.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czs.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wru.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kjz.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eip.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ego.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ico.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://thc.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://cso.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gvj.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://myl.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jci.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akl.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://coz.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://edp.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://xio.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://txc.vehdjk.com

[F04] 追加写入文件
来源：http://sfg.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kso.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hit.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pvc.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnj.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dcr.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://foq.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://krl.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uwt.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://uym.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qiy.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://jvp.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://ynm.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://vjl.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://har.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yhv.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://rtn.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://cxe.jinqigfzy.top

[F06] 删除文件
来源：http://mms.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://jdq.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://gpl.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://tas.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://owr.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kdx.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://zpf.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://sgh.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://hqo.tarul.cn

[F07] 创建目录（含多级）
来源：http://fqv.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lbv.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ryt.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rui.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vox.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kqe.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ara.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqd.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pxe.zhijiandao.cn

[F08] 遍历目录
来源：http://qfx.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqv.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ngd.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://mdx.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://olq.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sfi.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://nit.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://ucj.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://acx.ehwqpu.com

[F09] 获取文件大小
来源：http://zzp.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://zqb.aizwys.cn

PHP:  filesize("a.txt");
来源：http://omo.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://hzy.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://ayw.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kes.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wql.ybcxt.top

Ruby: File.size("a.txt")
来源：http://unh.jiagoushi.top

C#:   new FileInfo("a.txt").Length
来源：http://dyb.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://cak.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wtx.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ebh.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fud.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://qct.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tee.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ioz.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xhj.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xkw.ybcxt.top

[F11] 复制与移动文件
来源：http://ltn.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://umz.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hci.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://anw.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pyz.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ivi.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bty.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jwr.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yii.sweek.top

[F12] CSV 读写
来源：http://wpy.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zcq.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xkx.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://twv.52xcode.cn

TS:   // 同上
来源：http://fdg.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hed.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mhs.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vgt.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ihq.wangdashe.top

================================================================================
来源：http://xsb.yangfankeji.com

G. 面向对象
来源：http://vtp.ybcxt.top

================================================================================
来源：http://flx.nwbrower.top

[G01] 定义类
来源：http://cjz.yonumen.top

Py:   class User: pass
来源：http://xmb.tanke756.top

PHP:  class User {}
来源：http://wkn.jqgufenzy.top

JS:   class User {}
来源：http://ski.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://elw.wangdashe.top

Java: class User {}
来源：http://tjn.hammf.cn

Go:   type User struct { Name string }
来源：http://vbl.jqgufenzy.top

Ruby: class User; end
来源：http://vnn.redwolf501.top

C#:   class User {}
来源：http://crw.shanyushiyangtech.top

[G02] 构造函数
来源：http://ilf.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://dta.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://urd.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://eph.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://tmw.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://okz.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vys.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://sod.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://ytx.yuxming.cn

[G03] 实例属性
来源：http://qok.gzhubu.top

Py:   self.name = "x"
来源：http://opv.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://ufw.hysaishi.cn

JS:   this.name = "x";
来源：http://glr.hongshengwenyu.top

TS:   name: string = "x";
来源：http://lgi.xingfuxueyuan.xyz

Java: private String name;
来源：http://ism.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ona.nanxinkj.top

Ruby: @name = "x"
来源：http://mxg.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://tdg.svipenyu.cn

[G04] 定义方法
来源：http://pxz.redwolf501.top

Py:   def greet(self): return self.name
来源：http://fxj.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://biy.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://epb.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://xpo.ydzc1.top

Java: String greet() { return name; }
来源：http://pnb.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ndf.epnwcf.com

Ruby: def greet; @name; end
来源：http://tih.zycfv.cn

C#:   public string Greet() => Name;
来源：http://zpr.zdbjq.cn

[G05] 继承
来源：http://imp.ybcxt.top

Py:   class Admin(User): pass
来源：http://bes.yj20258.top

PHP:  class Admin extends User {}
来源：http://caz.yuxming.cn

JS:   class Admin extends User {}
来源：http://nrs.ivvv.top

TS:   class Admin extends User {}
来源：http://kcz.yuxming.cn

Java: class Admin extends User {}
来源：http://hww.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mka.tianlin.xyz

Ruby: class Admin < User; end
来源：http://jeb.cdnleiting.top

C#:   class Admin : User {}
来源：http://wtn.epnwcf.com

[G06] 重写方法
来源：http://yvd.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://yno.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tdf.sweek.top

JS:   greet() { return "admin"; }
来源：http://div.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://mxn.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://lzl.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hij.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://fhw.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://ctj.9152youxi.cn

[G07] 调用父类方法
来源：http://okf.gotoacloud.top

Py:   super().greet()
来源：http://roq.jinqigfzy.top

PHP:  parent::greet();
来源：http://pnv.wangshuangyany.cn

JS:   super.greet();
来源：http://qds.hesvh.cn

TS:   super.greet();
来源：http://gph.yfazqb.com

Java: super.greet();
来源：http://yae.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jsg.ehwqpu.com


<!-- 参考信息 -->