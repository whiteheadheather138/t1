代发 wailian999

PHP:  implode(",", $items);
来源：http://yos.shangyingyoupin.top

JS:   items.join(",")
来源：http://ozw.sxryk.cn

TS:   items.join(",")
来源：http://dhy.pengpengdd.cyou

Java: String.join(",", items)
来源：http://log.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://ase.zdqjudy.top

Ruby: items.join(",")
来源：http://hht.yj20258.top

C#:   string.Join(",", items)
来源：http://usu.jiagoushi.top

[E09] 去除所有空白字符
来源：http://arq.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://llf.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dra.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://ejp.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://sjc.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://shv.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jfi.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://nfd.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cmu.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://cng.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://esl.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ryl.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://eyv.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://bji.shuidangran.top

Java: String.format("%03d", 7)
来源：http://vog.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ull.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gpe.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jur.dashuyun.cn

[E11] 反转字符串
来源：http://jbb.fengsongda.top

Py:   s[::-1]
来源：http://mvr.haohaochexian.top

PHP:  strrev($s);
来源：http://puo.hammf.cn

JS:   [...s].reverse().join("")
来源：http://jxa.316326.xyz

TS:   [...s].reverse().join("")
来源：http://svr.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zqj.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://kzb.meibo888.top

Ruby: s.reverse
来源：http://jdd.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://kfl.fehbvm.com

[E12] 统计某字符出现次数
来源：http://quq.ybcxt.top

Py:   s.count("a")
来源：http://pkc.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://hyi.uphjek.com

JS:   s.split("a").length - 1
来源：http://yxy.yueranfly.top

TS:   s.split("a").length - 1
来源：http://zhf.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pkq.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://wdb.quarkkingdee.top

Ruby: s.count("a")
来源：http://trh.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://ioo.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://meo.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://nhx.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pkm.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://idt.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://efj.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ejm.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ngi.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://saq.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://joo.pycfn.com

[E14] URL 编码与 Base64
来源：http://zrd.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://avd.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rae.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cax.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fip.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wza.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ksn.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zfl.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zcj.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://hip.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zmt.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ewm.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lji.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cxr.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tih.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hto.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ckt.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nkk.nwbrower.top

[E16] 数字千分位
来源：http://rxd.pycfn.com

Py:   f"{1234567:,}"
来源：http://mti.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://zqt.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cme.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://evm.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aka.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://twr.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vvl.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://yzd.yj20258888.top

[E17] 首字母大写
来源：http://sbc.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pwf.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vre.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nsu.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lll.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ssu.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ulk.gotoacloud.top

Ruby: s.capitalize
来源：http://mjf.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pcz.havefunace.top

[E18] 模板占位符替换
来源：http://lmd.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ajb.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jew.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sxp.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://iqg.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vxf.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lai.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fas.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cmt.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://zhf.xuetiantiany.cn

Py:   s.splitlines()
来源：http://lis.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pci.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://htg.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://evm.yonumen.top

Java: s.lines().toList()
来源：http://ojw.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://aqq.jqgufenzy.top

Ruby: s.lines
来源：http://tkv.bbcook.cn

C#:   s.Split('\n')
来源：http://wet.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://rby.shzxlz.cn

Py:   if not s:
来源：http://rzx.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cee.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pqg.cqqwz.cn

TS:   if (s === "") {}
来源：http://sra.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://dkv.zhiwuduotai.top

Go:   if s == "" {}
来源：http://owt.aibaodan.cn

Ruby: if s.empty?
来源：http://jve.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nxc.yuanzhike.top

[E21] 超长截断加省略号
来源：http://jqw.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uwv.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qpk.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://orj.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ahv.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ezx.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://epg.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ktf.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggy.xylfe.cn

[E22] 字节长度与字符长度
来源：http://lqj.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mun.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmz.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tre.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzk.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://urh.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iql.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://nxv.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uid.gzhubu.top

================================================================================
来源：http://aiv.shuidangran.top

F. 文件与目录
来源：http://mvh.iojbl.cn

================================================================================
来源：http://egp.tianlin.xyz

[F01] 读取整个文件
来源：http://dlo.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qhd.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://omp.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bmb.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://abg.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rkb.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dqd.daria6918.cn

Ruby: File.read("a.txt")
来源：http://fug.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://kvj.sweek.top

[F02] 逐行读取文件
来源：http://eez.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dlf.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kmf.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqs.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wza.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uib.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lti.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fxu.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kcf.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://htd.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nxk.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fqa.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fby.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aia.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rco.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dmx.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://jsh.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://snx.yj20258.top

[F04] 追加写入文件
来源：http://cga.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rrv.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eua.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oyu.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jmu.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ghn.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://smu.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://osg.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qbd.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://xup.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://elt.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://lmo.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://gdk.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://iom.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mkc.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gvt.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://ecz.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://ydi.sufxvd.cn

[F06] 删除文件
来源：http://inc.316326.xyz

Py:   os.remove("a.txt")
来源：http://qmv.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://dfc.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://wnt.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://wyt.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://glm.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://ymh.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://ecg.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://lwi.daria6918.cn

[F07] 创建目录（含多级）
来源：http://wop.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tav.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://szh.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mwg.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zka.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tzo.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xjq.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xqk.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://foa.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://tju.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uat.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jox.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://wda.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://sog.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://noo.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xew.xuanzx.com

Ruby: Dir.children("dir")
来源：http://ypo.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://ftn.yueranfly.top

[F09] 获取文件大小
来源：http://sjc.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://dvt.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://oep.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://etl.yonumen.top

TS:   fs.statSync("a.txt").size
来源：http://xui.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://jdr.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gjv.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://hwz.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://muk.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://sod.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lnv.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vmu.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eyx.52xcode.cn

TS:   path.extname("a.txt")
来源：http://otg.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bsw.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bng.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://soq.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://txu.c1oappe.top

[F11] 复制与移动文件
来源：http://pgo.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gfz.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rlk.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ybx.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivv.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ouo.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://klh.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://avj.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cnh.tarul.cn

[F12] CSV 读写
来源：http://eky.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pnk.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uif.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yxu.epnwcf.com

TS:   // 同上
来源：http://ius.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ipb.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qzs.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cps.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ebc.yanxiufei.cn

================================================================================
来源：http://xru.vehdjk.com

G. 面向对象
来源：http://vhn.fengsongda.top

================================================================================
来源：http://vja.ivvv.top

[G01] 定义类
来源：http://apt.jinghuilouyu.cn

Py:   class User: pass
来源：http://vgc.uphjek.com

PHP:  class User {}
来源：http://koq.jiagoushi.top

JS:   class User {}
来源：http://yit.sweek.top

TS:   class User { name: string = ""; }
来源：http://myw.meibo888.top

Java: class User {}
来源：http://rpj.jqgfzy.top

Go:   type User struct { Name string }
来源：http://jbh.yuanzhike.top

Ruby: class User; end
来源：http://jko.c1oappe.top

C#:   class User {}
来源：http://jhv.cheryme.top

[G02] 构造函数
来源：http://run.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wny.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://vkh.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://epd.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://bkq.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://pav.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iwc.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://bwk.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://bfn.hnqzz.top

[G03] 实例属性
来源：http://yll.wangdashe.top

Py:   self.name = "x"
来源：http://piz.c1oappe.top

PHP:  public string $name = "x";
来源：http://zlg.cdnleiting.top

JS:   this.name = "x";
来源：http://jzu.yueranfly.top

TS:   name: string = "x";
来源：http://cxr.jinghuilouyu.cn

Java: private String name;
来源：http://sbl.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ctz.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://tas.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://zdc.shzxlz.cn

[G04] 定义方法
来源：http://ham.smart0.xyz

Py:   def greet(self): return self.name
来源：http://aey.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lub.yj20258888.top

JS:   greet() { return this.name; }
来源：http://lva.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://nxx.yj20258888.top

Java: String greet() { return name; }
来源：http://zdj.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://flh.cdnleiting.top

Ruby: def greet; @name; end
来源：http://zyy.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://wbv.iojbl.cn

[G05] 继承
来源：http://jno.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://isc.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://dct.daxiang520.top

JS:   class Admin extends User {}
来源：http://wpt.hammf.cn

TS:   class Admin extends User {}
来源：http://hea.hammf.cn

Java: class Admin extends User {}
来源：http://cgu.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pis.shuidangran.top

Ruby: class Admin < User; end
来源：http://dwz.hywenlv.cn

C#:   class Admin : User {}
来源：http://geh.yvedp.cn

[G06] 重写方法
来源：http://qyu.sweek.top

Py:   def greet(self): return "admin"
来源：http://zyq.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rel.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://rap.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://xqt.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://mel.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ehx.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://fzx.jianghu66.top


<!-- 参考信息 -->