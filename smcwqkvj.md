代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cns.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujl.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://juo.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://jyz.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://jft.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jpg.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://kqn.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rhm.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://mgv.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gqf.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mdo.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://zfi.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://tay.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://nga.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fgx.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sdk.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bgu.cashguo.top

[E11] 反转字符串
来源：http://gsy.sweek.top

Py:   s[::-1]
来源：http://msq.aibaodan.cn

PHP:  strrev($s);
来源：http://anx.ivvv.top

JS:   [...s].reverse().join("")
来源：http://udy.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://yvt.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://kjk.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kjs.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://ojg.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bjp.cashguo.top

[E12] 统计某字符出现次数
来源：http://xav.xylfe.cn

Py:   s.count("a")
来源：http://qkq.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://brv.daria6918.cn

JS:   s.split("a").length - 1
来源：http://yyb.smart0.xyz

TS:   s.split("a").length - 1
来源：http://zjz.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bws.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://jyg.ivvv.top

Ruby: s.count("a")
来源：http://qux.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://vyp.aizwys.cn

[E13] 逐字符遍历
来源：http://bue.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://nsb.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gnn.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mgf.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hrj.zhixingplan.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zxw.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fmb.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://aae.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uqu.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://nve.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://opn.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hrk.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tgq.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hzh.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://chk.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qwo.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lfc.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzp.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://fwt.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ion.jyoumei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kdh.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://doy.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ycn.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wgw.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ihl.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iwr.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://heh.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://xez.yj20258888.top

Py:   f"{1234567:,}"
来源：http://zlq.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://whk.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uut.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://alo.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dfx.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ixk.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://len.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://gtt.tarul.cn

[E17] 首字母大写
来源：http://vxk.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gbg.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jxd.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uwm.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vrk.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ivh.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nuh.0kj1m.cn

Ruby: s.capitalize
来源：http://vnc.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lwt.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://tfx.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qjb.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gij.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rth.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://trt.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xnn.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eaj.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://crg.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujz.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://lsx.chenlongwang.top

Py:   s.splitlines()
来源：http://gqx.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xgc.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://mtf.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://cnc.sufxvd.cn

Java: s.lines().toList()
来源：http://fqo.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://jqx.jianghu66.top

Ruby: s.lines
来源：http://llu.xuanzx.com

C#:   s.Split('\n')
来源：http://adq.yvedp.cn

[E20] 判断字符串是否为空
来源：http://ztt.316326.xyz

Py:   if not s:
来源：http://xqz.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rik.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iba.yj20258888.top

TS:   if (s === "") {}
来源：http://ysh.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://eth.sweek.top

Go:   if s == "" {}
来源：http://lye.andypj.xyz

Ruby: if s.empty?
来源：http://hwi.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aua.tian-w.cn

[E21] 超长截断加省略号
来源：http://mjf.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jag.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ant.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dfb.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hhu.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dwv.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://bhe.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vsi.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oad.yvedp.cn

[E22] 字节长度与字符长度
来源：http://esr.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://arp.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xnr.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://stu.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikn.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://byp.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ssm.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://nhm.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aik.sufxvd.cn

================================================================================
来源：http://jgc.tian-w.cn

F. 文件与目录
来源：http://ddi.ivvv.top

================================================================================
来源：http://jxj.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://ejm.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ulc.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://jbi.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ynn.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pnj.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://juu.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://odc.tarul.cn

Ruby: File.read("a.txt")
来源：http://mzd.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://ild.ctjpmb.com

[F02] 逐行读取文件
来源：http://qpe.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tuq.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cvs.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mes.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqh.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ovn.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hlw.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jpg.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uxf.havefunace.top

[F03] 写入文件（覆盖）
来源：http://usp.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ryy.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gny.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xru.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rfy.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oei.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uzy.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://rvo.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ghp.zhijiandao.cn

[F04] 追加写入文件
来源：http://xzu.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pts.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://svd.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bfa.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cdt.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ucu.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fzy.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xce.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dlg.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://nlf.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://njn.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://ssx.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://nbj.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://tvd.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lxc.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jsb.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://ghc.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://szz.ydzc1.top

[F06] 删除文件
来源：http://nzq.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://wqj.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://rnp.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://wzj.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://qqa.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gmy.havefunace.top

Go:   os.Remove("a.txt")
来源：http://uie.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://csx.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://inl.shuidangran.top

[F07] 创建目录（含多级）
来源：http://ljy.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ojs.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://een.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bjw.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rmr.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://brr.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wag.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wsw.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mtq.guannengcc.top

[F08] 遍历目录
来源：http://kec.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tal.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qyr.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://gyx.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://lwl.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://flm.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://opx.redwolf501.top

Ruby: Dir.children("dir")
来源：http://mss.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://bfk.hnqzz.top

[F09] 获取文件大小
来源：http://ege.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://xud.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://xzz.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://sqx.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://ike.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://npp.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hhq.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://phd.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://mnp.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://ilv.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ido.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ihk.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sqv.fengsongda.top

TS:   path.extname("a.txt")
来源：http://jfl.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oqn.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tmy.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gej.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rue.meibo888.top

[F11] 复制与移动文件
来源：http://qax.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xse.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ssu.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwy.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://faw.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zow.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mnt.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xpv.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fib.snrcjt.cn

[F12] CSV 读写
来源：http://jmj.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wqr.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://byq.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kuv.hysaishi.cn

TS:   // 同上
来源：http://cdt.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mrf.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zvy.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ruo.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kgr.sysykeji.top

================================================================================
来源：http://fzc.hnqzz.top

G. 面向对象
来源：http://xuf.xinyue.icu

================================================================================
来源：http://tsi.ctjpmb.com

[G01] 定义类
来源：http://szx.svipenyu.cn

Py:   class User: pass
来源：http://wwu.quarkkingdee.top

PHP:  class User {}
来源：http://bsw.zhijiandao.cn

JS:   class User {}
来源：http://jwk.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://ixy.ivvv.top

Java: class User {}
来源：http://hnz.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://rkv.gotoacloud.top

Ruby: class User; end
来源：http://rux.jqgufenzy.top

C#:   class User {}
来源：http://umv.0kj1m.cn

[G02] 构造函数
来源：http://dhz.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://wit.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://stp.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://wdt.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://spr.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://pup.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cpf.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://ktv.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://ass.ydjk.org.cn

[G03] 实例属性
来源：http://xcn.bjfxy.top

Py:   self.name = "x"
来源：http://fji.jyoumei.cn

PHP:  public string $name = "x";
来源：http://jba.xuetiantiany.cn

JS:   this.name = "x";
来源：http://epp.jyoumei.cn

TS:   name: string = "x";
来源：http://azn.sjlbkw.cn

Java: private String name;
来源：http://dks.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xfc.cqqwz.cn

Ruby: @name = "x"
来源：http://wmp.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://jga.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://caq.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://odp.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ieu.316326.xyz

JS:   greet() { return this.name; }
来源：http://zzb.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://btn.zdbjq.cn

Java: String greet() { return name; }
来源：http://vdl.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://egj.fengsongda.top

Ruby: def greet; @name; end
来源：http://oat.tian-w.cn

C#:   public string Greet() => Name;
来源：http://btu.xinyue.icu

[G05] 继承
来源：http://sox.gogol.net.cn

Py:   class Admin(User): pass
来源：http://tyl.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://qia.xziqi.cn

JS:   class Admin extends User {}
来源：http://wrt.xziqi.cn

TS:   class Admin extends User {}
来源：http://ccm.hesvh.cn

Java: class Admin extends User {}
来源：http://nym.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sqv.andypj.xyz

Ruby: class Admin < User; end
来源：http://qca.fengsongda.top

C#:   class Admin : User {}
来源：http://ogt.daxiang520.top

[G06] 重写方法
来源：http://vml.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://aen.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bea.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://clr.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://brb.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://mcq.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gmd.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://qmh.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://wyh.jianghu66.top

[G07] 调用父类方法
来源：http://dqy.dianchejie.cn

Py:   super().greet()
来源：http://hch.xinyue.icu

PHP:  parent::greet();
来源：http://bkt.yuanzhike.top

JS:   super.greet();
来源：http://uax.birdmap.top

TS:   super.greet();
来源：http://ovf.jqgufenzy.top

Java: super.greet();
来源：http://qbr.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fku.zdqjudy.top


<!-- 参考信息 -->