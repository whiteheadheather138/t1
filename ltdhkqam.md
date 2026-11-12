代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mtl.ybcxt.top

Ruby: items.join(",")
来源：http://kjc.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://dge.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://uzd.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hds.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lcc.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://dgy.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://vuu.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://tmo.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fqg.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pco.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xmq.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://tcu.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jwn.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sfc.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://cab.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://zwy.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://aqn.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://plv.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://scd.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rlz.sufxvd.cn

[E11] 反转字符串
来源：http://qew.gaohongyu789.top

Py:   s[::-1]
来源：http://mlj.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://yxd.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://vai.cheryme.top

TS:   [...s].reverse().join("")
来源：http://bgm.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cez.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://now.yj202588.top

Ruby: s.reverse
来源：http://cha.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://ppu.meibo888.top

[E12] 统计某字符出现次数
来源：http://fch.sufxvd.cn

Py:   s.count("a")
来源：http://sxx.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://vyg.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://inn.nwbrower.top

TS:   s.split("a").length - 1
来源：http://adb.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gto.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://zok.316326.xyz

Ruby: s.count("a")
来源：http://aih.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://shl.epnwcf.com

[E13] 逐字符遍历
来源：http://opa.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://srl.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ufy.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://hgg.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://yih.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://owk.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ujh.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jwc.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yrt.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://mzc.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lqe.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vhc.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://prc.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rjt.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zne.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://czn.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lxz.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tew.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://wxz.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://alp.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ykf.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://msr.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jut.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sxz.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oyb.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sht.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gxi.yj202588.top

[E16] 数字千分位
来源：http://svg.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://amg.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://mdm.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vhk.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qxr.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wnr.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tzh.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fig.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://rkw.bbcook.cn

[E17] 首字母大写
来源：http://wvk.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aqh.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://szs.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gpz.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fnj.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cpl.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bby.tianlin.xyz

Ruby: s.capitalize
来源：http://atb.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://amh.jqgufenzy.top

[E18] 模板占位符替换
来源：http://alu.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nku.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zpg.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cqv.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ckm.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tjn.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ayu.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sst.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qjd.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://zof.9152youxi.cn

Py:   s.splitlines()
来源：http://jcm.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lzk.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://xrm.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://qvx.cqqwz.cn

Java: s.lines().toList()
来源：http://epe.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://pqm.fehbvm.com

Ruby: s.lines
来源：http://lhu.zycfv.cn

C#:   s.Split('\n')
来源：http://ngq.redwolf501.top

[E20] 判断字符串是否为空
来源：http://byu.epnwcf.com

Py:   if not s:
来源：http://wdm.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tfm.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xmf.nanxinkj.top

TS:   if (s === "") {}
来源：http://zkl.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://tbu.jianghu66.top

Go:   if s == "" {}
来源：http://xgi.ivvv.top

Ruby: if s.empty?
来源：http://fqj.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nzk.wangdashe.top

[E21] 超长截断加省略号
来源：http://uhu.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ard.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://guc.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nln.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://acv.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fxv.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://lad.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lem.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zww.yueranfly.top

[E22] 字节长度与字符长度
来源：http://txa.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uxm.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfk.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pyp.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikn.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qpy.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qnb.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://xau.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qph.shzxlz.cn

================================================================================
来源：http://zbi.zhengqikj.top

F. 文件与目录
来源：http://kuc.jqgufenzy.top

================================================================================
来源：http://ctm.tanke756.top

[F01] 读取整个文件
来源：http://kzl.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rfb.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://gfb.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vcw.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cyh.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://twb.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rkj.uphjek.com

Ruby: File.read("a.txt")
来源：http://jhz.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://qmh.wangdashe.top

[F02] 逐行读取文件
来源：http://qhu.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndz.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jjt.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egf.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://klm.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://odv.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fzg.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ppi.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ypy.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://tvw.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hhr.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vbb.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://let.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ipc.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sye.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nlg.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://weo.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jxy.sxryk.cn

[F04] 追加写入文件
来源：http://mpr.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ftb.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oux.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wqp.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fyc.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ldw.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://spt.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tmf.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lem.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://afg.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vsx.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://ywj.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://wlt.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://jmd.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lqz.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uks.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://ron.316326.xyz

C#:   File.Exists("a.txt")
来源：http://tky.jqgufenzy.top

[F06] 删除文件
来源：http://clz.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://wvk.daxiang520.top

PHP:  unlink("a.txt");
来源：http://qem.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://oqf.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://yto.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sew.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://afy.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://qko.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://cqe.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://blf.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xsg.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gtq.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sda.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://osq.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bak.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mzk.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cfc.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fdr.zdqjudy.top

[F08] 遍历目录
来源：http://fhq.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eab.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ela.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://gso.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://moa.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ael.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jaa.yonumen.top

Ruby: Dir.children("dir")
来源：http://dwa.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://gwx.jqgfzy.top

[F09] 获取文件大小
来源：http://ecx.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://bvk.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://kss.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://bdi.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://bng.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://egs.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oxv.yuxming.cn

Ruby: File.size("a.txt")
来源：http://jup.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://cbr.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://hpa.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mvc.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gat.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lmc.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://btp.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uyd.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bnz.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rsn.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fsk.gogol.net.cn

[F11] 复制与移动文件
来源：http://wkm.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lrk.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://prm.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahf.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aeh.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mkg.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pyn.svipenyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zoc.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybd.gaohongyu789.top

[F12] CSV 读写
来源：http://skx.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://obs.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxl.yj20258888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jqh.fehbvm.com

TS:   // 同上
来源：http://rcn.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yzu.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hzc.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tno.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://whi.hywenlv.cn

================================================================================
来源：http://yhe.vehdjk.com

G. 面向对象
来源：http://ocz.jqgfzy.top

================================================================================
来源：http://tea.zhixingplan.top

[G01] 定义类
来源：http://lhx.daxiang520.top

Py:   class User: pass
来源：http://cxx.guowangkeji.top

PHP:  class User {}
来源：http://nog.hcnkem.com

JS:   class User {}
来源：http://rix.tarul.cn

TS:   class User { name: string = ""; }
来源：http://mym.ctjpmb.com

Java: class User {}
来源：http://dus.daria6918.cn

Go:   type User struct { Name string }
来源：http://rtb.sxryk.cn

Ruby: class User; end
来源：http://zaq.zdbjq.cn

C#:   class User {}
来源：http://kuz.hcnkem.com

[G02] 构造函数
来源：http://ddp.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://svs.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://tmg.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://mqb.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://opd.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://xel.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fjs.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://ele.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://czs.tarul.cn

[G03] 实例属性
来源：http://ekd.hnxiangtu.top

Py:   self.name = "x"
来源：http://xjw.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://zfg.chenzaomai.com

JS:   this.name = "x";
来源：http://fzb.tianlin.xyz

TS:   name: string = "x";
来源：http://stx.sweek.top

Java: private String name;
来源：http://uin.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eod.chenlongwang.top

Ruby: @name = "x"
来源：http://zne.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://dwc.uphjek.com

[G04] 定义方法
来源：http://yqk.sweek.top

Py:   def greet(self): return self.name
来源：http://pzi.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zpo.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://nan.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://sbq.zhixingplan.top

Java: String greet() { return name; }
来源：http://tvt.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmz.ydzc1.top

Ruby: def greet; @name; end
来源：http://xgf.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://def.shuidangran.top

[G05] 继承
来源：http://viv.zycfv.cn

Py:   class Admin(User): pass
来源：http://onw.52xcode.cn

PHP:  class Admin extends User {}
来源：http://wkg.haohaochexian.top

JS:   class Admin extends User {}
来源：http://acy.zycfv.cn

TS:   class Admin extends User {}
来源：http://ien.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://tnb.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://czb.fzhhl.top

Ruby: class Admin < User; end
来源：http://dxf.ivvv.top

C#:   class Admin : User {}
来源：http://hxh.quarkkingdee.top

[G06] 重写方法
来源：http://qzz.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://jrv.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yuv.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://tvw.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://flo.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jyv.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vxn.yonumen.top

Ruby: def greet; "admin"; end
来源：http://kas.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://tsi.zycfv.cn

[G07] 调用父类方法
来源：http://hwh.hongshengwenyu.top

Py:   super().greet()
来源：http://ikr.aizwys.cn

PHP:  parent::greet();
来源：http://ivk.vehdjk.com


<!-- 参考信息 -->