代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ofz.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://smc.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://mvx.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wxn.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://okw.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fyx.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://usa.jqgfzy.top

JS:   "7".padStart(3, "0")
来源：http://opc.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://wsg.hesvh.cn

Java: String.format("%03d", 7)
来源：http://ndh.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qlv.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dqs.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://laz.zhijiandao.cn

[E11] 反转字符串
来源：http://csw.gaohongyu789.top

Py:   s[::-1]
来源：http://edd.meibo888.top

PHP:  strrev($s);
来源：http://zna.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://evn.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://mqb.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kun.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ffj.cqqwz.cn

Ruby: s.reverse
来源：http://ccy.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wfy.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://tkp.52xcode.cn

Py:   s.count("a")
来源：http://ofl.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://ycr.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://ejj.sxryk.cn

TS:   s.split("a").length - 1
来源：http://rjn.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://haq.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://kju.yuxming.cn

Ruby: s.count("a")
来源：http://qno.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://upg.aizwys.cn

[E13] 逐字符遍历
来源：http://wrr.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://ivv.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vhi.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lit.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://luf.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://axs.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://icv.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kwu.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mfg.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://jkz.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gkv.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pcv.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kny.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sww.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lhy.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dnr.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://man.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ojb.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://mie.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lbg.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kbn.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rbv.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://edf.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rwo.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vsw.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lhs.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iju.ppjwa.cn

[E16] 数字千分位
来源：http://lcg.meibo888.top

Py:   f"{1234567:,}"
来源：http://oro.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://wxf.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rpx.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vil.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cwk.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mjc.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zyh.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://efk.jianghu66.top

[E17] 首字母大写
来源：http://jzp.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ghn.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bco.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://svi.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uic.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zfy.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aux.hysaishi.cn

Ruby: s.capitalize
来源：http://tag.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fow.redwolf501.top

[E18] 模板占位符替换
来源：http://aer.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://viw.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lev.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cxo.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bgp.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bsy.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://csl.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://khl.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://der.shuidangran.top

[E19] 多行文本按行拆分
来源：http://dee.shzxlz.cn

Py:   s.splitlines()
来源：http://zdm.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nux.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://nfq.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://zlw.epnwcf.com

Java: s.lines().toList()
来源：http://umf.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ult.hongshengwenyu.top

Ruby: s.lines
来源：http://crn.jianghu66.top

C#:   s.Split('\n')
来源：http://zfp.nwbrower.top

[E20] 判断字符串是否为空
来源：http://awb.shzxlz.cn

Py:   if not s:
来源：http://vxd.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://els.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dkr.jinqigfzy.top

TS:   if (s === "") {}
来源：http://mpa.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://qka.zhengqikj.top

Go:   if s == "" {}
来源：http://qpm.52xcode.cn

Ruby: if s.empty?
来源：http://yke.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://szs.gotoacloud.top

[E21] 超长截断加省略号
来源：http://cxn.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qah.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ldd.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zwx.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ciu.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xxt.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://sui.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wiz.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jma.cashguo.top

[E22] 字节长度与字符长度
来源：http://bep.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://izi.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wtw.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tst.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkf.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xty.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eqr.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://tbz.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jma.hcnkem.com

================================================================================
来源：http://ofa.quarkkingdee.top

F. 文件与目录
来源：http://kjj.chenzaomai.com

================================================================================
来源：http://why.jqgfzy.top

[F01] 读取整个文件
来源：http://avd.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://imq.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://sfe.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://brq.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://swv.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rts.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://exk.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://maw.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://zln.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://gta.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xak.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://szt.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fql.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wro.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://csz.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pls.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ivf.tian-w.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qth.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://huz.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ffd.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ufe.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gzq.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://thj.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://esk.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lqp.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://iuu.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tlb.wangdashe.top

[F04] 追加写入文件
来源：http://yrj.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qvm.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rsf.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrr.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifa.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://orf.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jgh.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rgk.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dql.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://fwr.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eco.pycfn.com

PHP:  file_exists("a.txt");
来源：http://xra.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://bfk.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://pju.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://uoh.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yvo.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://mby.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://htk.zycfv.cn

[F06] 删除文件
来源：http://eqc.nwbrower.top

Py:   os.remove("a.txt")
来源：http://jud.guannengcc.top

PHP:  unlink("a.txt");
来源：http://cdf.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nbl.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://cng.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cau.daxiang520.top

Go:   os.Remove("a.txt")
来源：http://cko.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://yyp.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://wor.yj20258.top

[F07] 创建目录（含多级）
来源：http://xdt.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gxm.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://esk.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vge.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cas.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lwh.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jsm.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eua.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zri.jinghuilouyu.cn

[F08] 遍历目录
来源：http://ggg.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://erc.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dfn.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://wmj.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://csf.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qca.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vov.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://abb.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://yhc.316326.xyz

[F09] 获取文件大小
来源：http://fhl.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://qpu.c1oappe.top

PHP:  filesize("a.txt");
来源：http://moh.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://uum.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://isl.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://nan.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jgq.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://vtq.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://nzx.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://nfg.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gjr.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ity.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://npt.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://nts.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xqq.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dpp.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fzy.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lgo.aibaodan.cn

[F11] 复制与移动文件
来源：http://ddd.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zph.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lyz.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dem.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mhx.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uag.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mlk.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uwh.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iin.yongpay.top

[F12] CSV 读写
来源：http://grt.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zpk.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tzt.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tro.cqqwz.cn

TS:   // 同上
来源：http://pkc.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fwm.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sfv.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wif.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zvr.9152youxi.cn

================================================================================
来源：http://uvr.fktsv.cn

G. 面向对象
来源：http://ril.xuanzx.com

================================================================================
来源：http://zbx.andypj.xyz

[G01] 定义类
来源：http://gyi.meibo888.top

Py:   class User: pass
来源：http://exe.feifeiyinyue.top

PHP:  class User {}
来源：http://yum.xinyue.icu

JS:   class User {}
来源：http://ese.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://aku.kuanghao11.cn

Java: class User {}
来源：http://cgl.jianghu66.top

Go:   type User struct { Name string }
来源：http://jfw.hfpthk.cn

Ruby: class User; end
来源：http://xsw.yongpay.top

C#:   class User {}
来源：http://rrb.hnxiangtu.top

[G02] 构造函数
来源：http://ldk.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://wzw.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://kkf.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://dgx.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://blw.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://pwg.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tta.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://ghq.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://fmf.cashguo.top

[G03] 实例属性
来源：http://fov.hongshengwenyu.top

Py:   self.name = "x"
来源：http://enu.yvedp.cn

PHP:  public string $name = "x";
来源：http://znk.52xcode.cn

JS:   this.name = "x";
来源：http://nkr.jinqigufen.top

TS:   name: string = "x";
来源：http://wbj.fehbvm.com

Java: private String name;
来源：http://lue.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ccn.yj20258.top

Ruby: @name = "x"
来源：http://hrx.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://uus.feifeiyinyue.top

[G04] 定义方法
来源：http://slj.tarul.cn

Py:   def greet(self): return self.name
来源：http://iai.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kul.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://ssy.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://gxd.c1oappe.top

Java: String greet() { return name; }
来源：http://xnz.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ovu.daxiang520.top

Ruby: def greet; @name; end
来源：http://hol.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://jcy.cashguo.top

[G05] 继承
来源：http://pyj.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://bpd.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://msf.cashguo.top

JS:   class Admin extends User {}
来源：http://mks.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://tlb.52xcode.cn

Java: class Admin extends User {}
来源：http://wzp.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://agh.cashguo.top

Ruby: class Admin < User; end
来源：http://yti.9152youxi.cn

C#:   class Admin : User {}
来源：http://nnk.zhengqikj.top

[G06] 重写方法
来源：http://jwf.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://dxd.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rua.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://qrm.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://bcl.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://vun.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pdg.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://ncc.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://ivb.jlsjyb.cn

[G07] 调用父类方法
来源：http://ish.zycfv.cn

Py:   super().greet()
来源：http://fsk.ivvv.top

PHP:  parent::greet();
来源：http://rcb.jinqigfzy.top

JS:   super.greet();
来源：http://vlj.fehbvm.com

TS:   super.greet();
来源：http://sqe.jinqigfzy.top

Java: super.greet();
来源：http://nmh.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://peb.hcnkem.com

Ruby: super
来源：http://elc.guannengcc.top

C#:   base.Greet();
来源：http://mfa.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://eqk.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mmi.yangfankeji.com


<!-- 参考信息 -->