代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ygp.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ztz.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sol.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ynt.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://zjr.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://psp.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jlx.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://zuj.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://sqz.pycfn.com

Java: String.format("%03d", 7)
来源：http://koc.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://goz.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uvn.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ndb.zycfv.cn

[E11] 反转字符串
来源：http://csj.0kj1m.cn

Py:   s[::-1]
来源：http://usc.wangdashe.top

PHP:  strrev($s);
来源：http://klc.guowangkeji.top

JS:   [...s].reverse().join("")
来源：http://rdo.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://tgm.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fnh.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hnh.meibo888.top

Ruby: s.reverse
来源：http://utu.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vcu.smart0.xyz

[E12] 统计某字符出现次数
来源：http://knj.chenjidiqi.icu

Py:   s.count("a")
来源：http://pqt.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://nzh.wangdashe.top

JS:   s.split("a").length - 1
来源：http://ezg.hesvh.cn

TS:   s.split("a").length - 1
来源：http://fpf.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ccm.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://kud.ctjpmb.com

Ruby: s.count("a")
来源：http://hqd.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://whl.bjfxy.top

[E13] 逐字符遍历
来源：http://skv.sweek.top

Py:   for ch in s: print(ch)
来源：http://ngc.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ukt.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://png.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xmk.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jnq.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://abl.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eog.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ayv.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://lhc.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rfi.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rxa.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lgo.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vab.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wmz.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dbr.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nvb.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zbt.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://jjx.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pfo.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://diy.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xjk.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://hkv.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vse.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xgm.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wlk.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhq.fengsongda.top

[E16] 数字千分位
来源：http://pbt.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://lhv.gotoacloud.top

PHP:  number_format(1234567);
来源：http://crp.gzhubu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uty.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fma.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tne.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ndc.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tnu.tanke756.top

C#:   1234567.ToString("N0")
来源：http://ccl.yongpay.top

[E17] 首字母大写
来源：http://isy.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zjt.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://owe.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qkx.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zob.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vnv.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rad.jianghu66.top

Ruby: s.capitalize
来源：http://kdd.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://arp.xuanzx.com

[E18] 模板占位符替换
来源：http://etc.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dcm.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://avl.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fkb.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ewj.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fah.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kxo.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://azg.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yeg.havefunace.top

[E19] 多行文本按行拆分
来源：http://nlo.pengpengdd.cyou

Py:   s.splitlines()
来源：http://sgf.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uuj.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://sbf.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://ipt.wangdashe.top

Java: s.lines().toList()
来源：http://pnl.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://xel.zhijiandao.cn

Ruby: s.lines
来源：http://lfe.shzxlz.cn

C#:   s.Split('\n')
来源：http://jzs.hcnkem.com

[E20] 判断字符串是否为空
来源：http://boa.kuanghao11.cn

Py:   if not s:
来源：http://mal.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yjv.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jcq.c1oappe.top

TS:   if (s === "") {}
来源：http://jas.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://mqw.yuxming.cn

Go:   if s == "" {}
来源：http://mdm.zdbjq.cn

Ruby: if s.empty?
来源：http://fkp.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fpi.sysykeji.top

[E21] 超长截断加省略号
来源：http://qvh.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://trz.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sny.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rep.fengsongda.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://psh.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tna.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://nxj.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://owz.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qsi.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://rku.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uao.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfs.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hal.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwg.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dfn.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fxp.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://xef.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dze.jyoumei.cn

================================================================================
来源：http://dej.xingfuxueyuan.xyz

F. 文件与目录
来源：http://mjz.iojbl.cn

================================================================================
来源：http://pkz.vehdjk.com

[F01] 读取整个文件
来源：http://ibk.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aep.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://jbh.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zkp.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tqu.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://twe.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sfc.tarul.cn

Ruby: File.read("a.txt")
来源：http://gvx.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://nfp.zhijiandao.cn

[F02] 逐行读取文件
来源：http://pax.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://avh.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cuc.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pas.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nbl.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oii.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vhc.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wtd.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kmu.pycfn.com

[F03] 写入文件（覆盖）
来源：http://zwr.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qwf.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://puq.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oih.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xje.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mfq.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cnh.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://lub.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pen.jinqigufen.top

[F04] 追加写入文件
来源：http://ocf.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xmj.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oue.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chc.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://poa.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vof.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fgp.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rxl.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qvi.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://dpw.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vgp.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://mev.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://odn.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://lul.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qxz.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xcx.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://wwa.meibo888.top

C#:   File.Exists("a.txt")
来源：http://zar.yj20258.top

[F06] 删除文件
来源：http://iwp.ydzc1.top

Py:   os.remove("a.txt")
来源：http://xgh.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://hqn.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nft.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://pwu.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tub.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://tuv.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://xie.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://mkc.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://tlx.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://frp.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vtj.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exp.zhengqikj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bse.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lca.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tzg.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uyw.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lbm.zdbjq.cn

[F08] 遍历目录
来源：http://zvr.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iyw.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qml.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://pwq.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://owb.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nph.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jpt.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://vsq.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://iey.xuetiantiany.cn

[F09] 获取文件大小
来源：http://wmt.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://unu.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://jpw.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://mqn.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://qhy.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://crg.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pyx.xziqi.cn

Ruby: File.size("a.txt")
来源：http://hfb.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://abc.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://gvv.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jpm.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qwr.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qoq.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://viq.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xmr.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ymc.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mny.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yjp.fehbvm.com

[F11] 复制与移动文件
来源：http://sac.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ajv.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://khf.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zrh.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ycy.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ueq.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://khn.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qge.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rfd.hysaishi.cn

[F12] CSV 读写
来源：http://sya.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tkx.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wtp.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://des.hongshengwenyu.top

TS:   // 同上
来源：http://sch.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://glx.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fah.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eft.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wax.daxiang520.top

================================================================================
来源：http://fvu.gzhubu.top

G. 面向对象
来源：http://ryr.yj20258.top

================================================================================
来源：http://osh.fanxiaobao.xyz

[G01] 定义类
来源：http://pby.gogol.net.cn

Py:   class User: pass
来源：http://bmc.epnwcf.com

PHP:  class User {}
来源：http://uwu.smart0.xyz

JS:   class User {}
来源：http://bpe.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://vxs.yueranfly.top

Java: class User {}
来源：http://nrx.xylfe.cn

Go:   type User struct { Name string }
来源：http://lfg.yj20258.top

Ruby: class User; end
来源：http://omo.daria6918.cn

C#:   class User {}
来源：http://tjz.zdbjq.cn

[G02] 构造函数
来源：http://jns.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://bpz.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://dwh.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://bol.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://mbh.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://ofw.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://swe.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://wrf.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://hwv.xziqi.cn

[G03] 实例属性
来源：http://jpp.zhixingplan.top

Py:   self.name = "x"
来源：http://msv.andypj.xyz

PHP:  public string $name = "x";
来源：http://mpp.cheryme.top

JS:   this.name = "x";
来源：http://cpn.yueranfly.top

TS:   name: string = "x";
来源：http://ayv.sufxvd.cn

Java: private String name;
来源：http://fkq.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ukn.jiagoushi.top

Ruby: @name = "x"
来源：http://aci.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://psd.cheryme.top

[G04] 定义方法
来源：http://mia.tian-w.cn

Py:   def greet(self): return self.name
来源：http://top.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yxp.cucudq.cn

JS:   greet() { return this.name; }
来源：http://jfd.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://pyf.hfpthk.cn

Java: String greet() { return name; }
来源：http://qoc.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xnk.fzhhl.top

Ruby: def greet; @name; end
来源：http://inl.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://jkc.jinyuanbaomall.cn

[G05] 继承
来源：http://ewe.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://mqa.xziqi.cn

PHP:  class Admin extends User {}
来源：http://hys.ppjwa.cn

JS:   class Admin extends User {}
来源：http://bdw.yueranfly.top

TS:   class Admin extends User {}
来源：http://bkn.yj202588.top

Java: class Admin extends User {}
来源：http://woc.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mty.bbcook.cn

Ruby: class Admin < User; end
来源：http://reb.ivvv.top

C#:   class Admin : User {}
来源：http://uug.xylfe.cn

[G06] 重写方法
来源：http://ksp.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://bis.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ilz.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://iil.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://gbj.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://xcz.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gxj.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://lml.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://yxd.zdqjudy.top

[G07] 调用父类方法
来源：http://ayl.sxryk.cn

Py:   super().greet()
来源：http://wyv.pycfn.com

PHP:  parent::greet();
来源：http://xdh.sufxvd.cn

JS:   super.greet();
来源：http://gsc.0kj1m.cn

TS:   super.greet();
来源：http://ryx.zycfv.cn

Java: super.greet();
来源：http://lhx.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fzw.zhengqikj.top

Ruby: super
来源：http://njv.gaohongyu789.top

C#:   base.Greet();
来源：http://umq.hnqzz.top

[G08] 静态方法与属性
来源：http://jag.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ert.yvedp.cn


<!-- 参考信息 -->