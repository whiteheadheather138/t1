代发 wailian999

Ruby: s.split(",");  s.split
来源：http://eis.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dlt.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://xmy.gotoacloud.top

Py:   ",".join(items)
来源：http://jbe.shuidangran.top

PHP:  implode(",", $items);
来源：http://wjh.wangdashe.top

JS:   items.join(",")
来源：http://syx.haohaochexian.top

TS:   items.join(",")
来源：http://ikr.meibo888.top

Java: String.join(",", items)
来源：http://nyx.tanke756.top

Go:   strings.Join(items, ",")
来源：http://ajl.dashuyun.cn

Ruby: items.join(",")
来源：http://slh.ybcxt.top

C#:   string.Join(",", items)
来源：http://oww.ctjpmb.com

[E09] 去除所有空白字符
来源：http://juw.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rqx.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpp.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://xuc.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://lga.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://gte.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://irw.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eje.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gxz.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://pba.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ehr.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://myc.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://nye.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://xwc.yongpay.top

Java: String.format("%03d", 7)
来源：http://ydz.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://for.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mdr.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nec.52xcode.cn

[E11] 反转字符串
来源：http://rwd.haohaochexian.top

Py:   s[::-1]
来源：http://xgz.yanxiufei.cn

PHP:  strrev($s);
来源：http://izi.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://jrf.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://nrv.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://azq.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgm.xylfe.cn

Ruby: s.reverse
来源：http://fiy.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://hvd.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://jpu.redwolf501.top

Py:   s.count("a")
来源：http://omo.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://bni.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://jyh.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://ypp.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cnw.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://nxn.zycfv.cn

Ruby: s.count("a")
来源：http://ych.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://uhd.sjlbkw.cn

[E13] 逐字符遍历
来源：http://vab.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://ipp.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jzm.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hgd.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rmq.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yrk.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://avu.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lnn.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cbg.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://oku.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vdk.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wxu.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gcb.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ait.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ypd.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ydf.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ppc.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vrx.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://wtl.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mwx.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fyr.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qfl.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zme.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kpd.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xda.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://owh.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cbl.yuxming.cn

[E16] 数字千分位
来源：http://phq.tian-w.cn

Py:   f"{1234567:,}"
来源：http://szb.daxiang520.top

PHP:  number_format(1234567);
来源：http://wui.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kfl.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mxo.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yit.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zlz.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://syy.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://bxc.zhijiandao.cn

[E17] 首字母大写
来源：http://wzj.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dvv.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yoy.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nyq.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://stq.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pin.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cfp.chenlongwang.top

Ruby: s.capitalize
来源：http://dsi.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fop.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://qgr.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pei.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://biu.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sze.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rdc.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ygv.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://auc.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xxz.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gwn.yfazqb.com

[E19] 多行文本按行拆分
来源：http://qdx.c1oappe.top

Py:   s.splitlines()
来源：http://tle.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kyx.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://glh.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://tqn.yuxming.cn

Java: s.lines().toList()
来源：http://vpp.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://tpt.vehdjk.com

Ruby: s.lines
来源：http://tpm.daxiang520.top

C#:   s.Split('\n')
来源：http://uoj.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://nat.hnqzz.top

Py:   if not s:
来源：http://avo.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vin.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yxq.epnwcf.com

TS:   if (s === "") {}
来源：http://qib.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://ytm.yuxming.cn

Go:   if s == "" {}
来源：http://emc.svipenyu.cn

Ruby: if s.empty?
来源：http://qem.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kws.yfazqb.com

[E21] 超长截断加省略号
来源：http://bew.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qgw.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vew.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vrm.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xkv.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://klc.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://saw.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fon.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dud.iojbl.cn

[E22] 字节长度与字符长度
来源：http://mdj.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://juu.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cks.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://csx.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uzc.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sqd.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oia.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://mne.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pug.yangfankeji.com

================================================================================
来源：http://ccb.kuanghao11.cn

F. 文件与目录
来源：http://rqa.xingfuxueyuan.xyz

================================================================================
来源：http://akg.quarkkingdee.top

[F01] 读取整个文件
来源：http://luf.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://geb.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://efo.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uei.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ngv.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xgw.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uza.daria6918.cn

Ruby: File.read("a.txt")
来源：http://gaa.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://fge.dashuyun.cn

[F02] 逐行读取文件
来源：http://mcg.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zgg.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eqx.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://val.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pgf.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ntp.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bli.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vri.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://usl.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://ekw.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ovp.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tux.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://trf.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yhw.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wwj.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yfo.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://lvs.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qzj.yanxiufei.cn

[F04] 追加写入文件
来源：http://scj.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mac.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mqg.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xxm.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://voe.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ztq.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tmz.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lws.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zbp.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://rso.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mnk.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://kpc.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://buf.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://yfd.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fjw.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zac.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://dmx.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://mhs.uphjek.com

[F06] 删除文件
来源：http://nfw.hesvh.cn

Py:   os.remove("a.txt")
来源：http://huj.xylfe.cn

PHP:  unlink("a.txt");
来源：http://fhb.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://rpj.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://czm.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eud.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://pxg.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://lsj.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://dbp.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://hvj.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://les.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://isz.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ref.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pdf.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://khp.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://igw.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://myt.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://goa.gzhubu.top

[F08] 遍历目录
来源：http://zvz.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pad.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zkd.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://fcq.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://inp.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bfn.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tnt.ybcxt.top

Ruby: Dir.children("dir")
来源：http://shv.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://ymf.guowangkeji.top

[F09] 获取文件大小
来源：http://jcn.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://aof.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://lcz.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://ymi.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://qca.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://izm.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jwl.sysykeji.top

Ruby: File.size("a.txt")
来源：http://zlj.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://pee.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://kwq.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kep.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://atx.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vma.shuidangran.top

TS:   path.extname("a.txt")
来源：http://xll.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iwm.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cuv.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wfu.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jgr.9152youxi.cn

[F11] 复制与移动文件
来源：http://xjd.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zjn.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vjl.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://inv.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uqv.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fle.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ynw.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zhv.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fad.nanxinkj.top

[F12] CSV 读写
来源：http://fbs.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lzp.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cvf.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iqu.ywan-chungtsiang.top

TS:   // 同上
来源：http://gvd.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tka.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cjr.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lus.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tre.yuanzhike.top

================================================================================
来源：http://vtt.jlsjyb.cn

G. 面向对象
来源：http://pke.guowangkeji.top

================================================================================
来源：http://mrh.shangyingyoupin.top

[G01] 定义类
来源：http://clz.ivvv.top

Py:   class User: pass
来源：http://yyp.9152youxi.cn

PHP:  class User {}
来源：http://mzo.wangdashe.top

JS:   class User {}
来源：http://yho.yonumen.top

TS:   class User { name: string = ""; }
来源：http://vek.yueranfly.top

Java: class User {}
来源：http://uft.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://njx.shzxlz.cn

Ruby: class User; end
来源：http://xlc.jinqigfzy.top

C#:   class User {}
来源：http://wpn.cheryme.top

[G02] 构造函数
来源：http://piv.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://ncu.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://ybg.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://cjo.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://uom.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://btj.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://adp.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://hpk.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://whi.cdnleiting.top

[G03] 实例属性
来源：http://seg.birdmap.top

Py:   self.name = "x"
来源：http://xqr.jianghu66.top

PHP:  public string $name = "x";
来源：http://qif.uphjek.com

JS:   this.name = "x";
来源：http://jdy.ydzc1.top

TS:   name: string = "x";
来源：http://luk.zhoulong.xyz

Java: private String name;
来源：http://xct.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oym.tian-w.cn

Ruby: @name = "x"
来源：http://fct.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://rgy.ybcxt.top

[G04] 定义方法
来源：http://dec.jianghu66.top

Py:   def greet(self): return self.name
来源：http://xps.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sdq.52xcode.cn

JS:   greet() { return this.name; }
来源：http://lys.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://jyx.wangdashe.top

Java: String greet() { return name; }
来源：http://nte.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mkc.shuidangran.top

Ruby: def greet; @name; end
来源：http://dpr.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://glp.mhx1999.top

[G05] 继承
来源：http://cpx.tanke756.top

Py:   class Admin(User): pass
来源：http://upt.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://agu.guannengcc.top

JS:   class Admin extends User {}
来源：http://rkb.epnwcf.com

TS:   class Admin extends User {}
来源：http://djp.haohaochexian.top

Java: class Admin extends User {}
来源：http://tfi.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eud.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://ngn.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://zlm.ppjwa.cn

[G06] 重写方法
来源：http://foz.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://xvj.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cqc.pycfn.com

JS:   greet() { return "admin"; }
来源：http://twd.cheryme.top


<!-- 参考信息 -->