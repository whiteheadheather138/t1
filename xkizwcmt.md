代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hma.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zdi.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://djf.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://wod.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://kvn.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dfv.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ara.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lam.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://fyg.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zlm.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://czl.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://swg.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://msb.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://iev.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://pjj.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rtq.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cnw.uphjek.com

[E11] 反转字符串
来源：http://mgo.shangyingyoupin.top

Py:   s[::-1]
来源：http://ehl.zhongyouzk.top

PHP:  strrev($s);
来源：http://vye.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://byx.yongpay.top

TS:   [...s].reverse().join("")
来源：http://dgn.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://oib.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xmm.zhoulong.xyz

Ruby: s.reverse
来源：http://auh.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://dyk.ybcxt.top

[E12] 统计某字符出现次数
来源：http://onn.zdbjq.cn

Py:   s.count("a")
来源：http://gsr.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://kru.shuidangran.top

JS:   s.split("a").length - 1
来源：http://lko.yj20258888.top

TS:   s.split("a").length - 1
来源：http://zwb.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://abi.uphjek.com

Go:   strings.Count(s, "a")
来源：http://wbh.gaohongyu789.top

Ruby: s.count("a")
来源：http://vbe.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://jgn.yj202588.top

[E13] 逐字符遍历
来源：http://ilm.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://kwe.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jqb.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kgd.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gat.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fwu.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mhk.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jej.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mnd.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://xni.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ugl.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://geb.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://irv.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yzv.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tfg.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tos.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xob.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://owd.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://czi.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zlh.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://edv.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kiv.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jcp.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zqh.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lag.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dae.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://djq.fzhhl.top

[E16] 数字千分位
来源：http://eqc.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://lpb.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://qfy.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kbp.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://gmf.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://seo.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://foy.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ogr.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://tna.aibaodan.cn

[E17] 首字母大写
来源：http://qeg.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aai.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rth.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://irz.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nmz.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://put.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://isu.zhengqikj.top

Ruby: s.capitalize
来源：http://ogh.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bun.yj202588.top

[E18] 模板占位符替换
来源：http://hnr.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gei.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zjz.dianchejie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gvl.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mwt.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zvl.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://btz.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ede.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mhl.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://nen.vehdjk.com

Py:   s.splitlines()
来源：http://uzy.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ept.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://itq.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://lsf.sjlbkw.cn

Java: s.lines().toList()
来源：http://jgw.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://kwu.316326.xyz

Ruby: s.lines
来源：http://kde.chenzaomai.com

C#:   s.Split('\n')
来源：http://srz.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://rhw.jinqigufen.top

Py:   if not s:
来源：http://jkr.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ahw.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lwg.ivvv.top

TS:   if (s === "") {}
来源：http://ayz.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://hqf.jiagoushi.top

Go:   if s == "" {}
来源：http://ypw.zhiwuduotai.top

Ruby: if s.empty?
来源：http://qtm.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://flb.zdbjq.cn

[E21] 超长截断加省略号
来源：http://mah.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lzs.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://suo.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sua.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mgp.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ajz.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://caf.jyoumei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kdn.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qtg.andypj.xyz

[E22] 字节长度与字符长度
来源：http://usm.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zjb.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jcb.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzi.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hjs.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xzt.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kxx.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://pfp.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jig.snrcjt.cn

================================================================================
来源：http://kht.chenjidiqi.icu

F. 文件与目录
来源：http://sil.jinqigfzy.top

================================================================================
来源：http://uqd.ctjpmb.com

[F01] 读取整个文件
来源：http://vyp.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wrn.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://rao.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ssj.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://czc.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kwz.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mxb.epnwcf.com

Ruby: File.read("a.txt")
来源：http://jne.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://khj.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://nda.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qnf.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qcn.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dzu.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aoo.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fen.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yai.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rtt.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kff.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://tov.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hsi.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hbl.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://flz.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cyq.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pzp.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gfh.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://qed.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ggt.chenlongwang.top

[F04] 追加写入文件
来源：http://xsk.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ckn.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xqc.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pry.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bqt.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ydp.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fjz.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fuh.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cns.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://fdy.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nux.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://suw.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://lxo.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://crs.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gnt.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nny.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://wxe.ivvv.top

C#:   File.Exists("a.txt")
来源：http://gwg.gaohongyu789.top

[F06] 删除文件
来源：http://mxk.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://atp.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://jwk.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://ogb.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eks.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dzv.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://jmw.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://vad.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://lie.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://wak.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sic.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://egt.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfj.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://apb.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zsg.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nrl.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fjp.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tqq.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://fhi.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jyq.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xuz.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://afi.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://wsd.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wof.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jie.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://kvt.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://roj.jqgfzy.top

[F09] 获取文件大小
来源：http://qmx.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://yvs.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://uxn.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://hyd.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://cyc.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://loi.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mqd.jianghu66.top

Ruby: File.size("a.txt")
来源：http://zxg.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://rlq.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://saj.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mul.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eik.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yjn.jianghu66.top

TS:   path.extname("a.txt")
来源：http://jjz.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hgq.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lqq.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ooa.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://atf.yj20258.top

[F11] 复制与移动文件
来源：http://oxd.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jsz.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pwp.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iob.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ibo.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://exc.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cey.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ups.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vqw.jinghuilouyu.cn

[F12] CSV 读写
来源：http://qin.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bms.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qfw.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uod.haohaochexian.top

TS:   // 同上
来源：http://jcr.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rrv.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lbk.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blb.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fko.bbcook.cn

================================================================================
来源：http://erj.yuanzhike.top

G. 面向对象
来源：http://pig.shangyingyoupin.top

================================================================================
来源：http://rjd.bbcook.cn

[G01] 定义类
来源：http://ros.tianlin.xyz

Py:   class User: pass
来源：http://ajx.chenjidiqi.icu

PHP:  class User {}
来源：http://mny.316326.xyz

JS:   class User {}
来源：http://qyh.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://gmj.yfazqb.com

Java: class User {}
来源：http://vxk.uphjek.com

Go:   type User struct { Name string }
来源：http://tat.yueranfly.top

Ruby: class User; end
来源：http://cej.zhengqikj.top

C#:   class User {}
来源：http://qvf.cqqwz.cn

[G02] 构造函数
来源：http://nwi.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://jnf.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://fju.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://osq.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://euq.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://rry.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hyx.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://cql.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://akw.nanxuanxn.top

[G03] 实例属性
来源：http://bbh.jlsjyb.cn

Py:   self.name = "x"
来源：http://lbu.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://ubx.aizwys.cn

JS:   this.name = "x";
来源：http://aeg.zdqjudy.top

TS:   name: string = "x";
来源：http://nwq.mhx1999.top

Java: private String name;
来源：http://rzx.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eyu.ydjk.org.cn

Ruby: @name = "x"
来源：http://rew.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://yaf.nanxinkj.top

[G04] 定义方法
来源：http://oco.sysykeji.top

Py:   def greet(self): return self.name
来源：http://kcd.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nlx.pycfn.com

JS:   greet() { return this.name; }
来源：http://scl.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://cjz.fengsongda.top

Java: String greet() { return name; }
来源：http://wuh.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lub.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://jxh.pycfn.com

C#:   public string Greet() => Name;
来源：http://clz.yuxming.cn

[G05] 继承
来源：http://jjm.fzhhl.top

Py:   class Admin(User): pass
来源：http://vnq.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://wye.birdmap.top

JS:   class Admin extends User {}
来源：http://lck.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://sjy.nanxinkj.top

Java: class Admin extends User {}
来源：http://sjh.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://exz.guowangkeji.top

Ruby: class Admin < User; end
来源：http://jly.smart0.xyz

C#:   class Admin : User {}
来源：http://ita.fengsongda.top

[G06] 重写方法
来源：http://fmh.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://vav.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gem.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://plu.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://eve.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://tbo.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eoi.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://qeh.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://ofb.zhengqikj.top

[G07] 调用父类方法
来源：http://hnt.dashuyun.cn

Py:   super().greet()
来源：http://aps.hfpthk.cn

PHP:  parent::greet();
来源：http://rhu.jqgufenzy.top

JS:   super.greet();
来源：http://xzj.hnqzz.top

TS:   super.greet();
来源：http://jbv.ppjwa.cn

Java: super.greet();
来源：http://isb.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eab.yanxiufei.cn


<!-- 参考信息 -->