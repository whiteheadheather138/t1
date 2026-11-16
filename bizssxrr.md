代发 wailian999

[E06] 替换子串
来源：http://elo.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ejg.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://ejx.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iuk.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://wxc.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yqr.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cwm.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kmu.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://jdh.yj20258888.top

[E07] 按分隔符拆分
来源：http://oeh.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oat.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://doc.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kmp.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://bxp.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://all.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ule.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://tve.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qji.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://ucd.cqqwz.cn

Py:   ",".join(items)
来源：http://pjk.sxryk.cn

PHP:  implode(",", $items);
来源：http://eki.ydzc1.top

JS:   items.join(",")
来源：http://vnp.fengsongda.top

TS:   items.join(",")
来源：http://nhy.guannengcc.top

Java: String.join(",", items)
来源：http://skt.tian-w.cn

Go:   strings.Join(items, ",")
来源：http://vjb.yj20258.top

Ruby: items.join(",")
来源：http://fze.9152youxi.cn

C#:   string.Join(",", items)
来源：http://ott.yuanzhike.top

[E09] 去除所有空白字符
来源：http://gdl.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xpz.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cxa.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://wky.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://ars.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://mlz.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dei.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zcw.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://efa.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://uyu.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://igi.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rhb.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://znc.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://zxv.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://fcr.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tiy.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hop.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pdz.bjfxy.top

[E11] 反转字符串
来源：http://sky.cashguo.top

Py:   s[::-1]
来源：http://ukp.birdmap.top

PHP:  strrev($s);
来源：http://zya.uphjek.com

JS:   [...s].reverse().join("")
来源：http://hdo.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://jjq.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://xli.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tec.andypj.xyz

Ruby: s.reverse
来源：http://kmb.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://bds.bjfxy.top

[E12] 统计某字符出现次数
来源：http://uuw.cqqwz.cn

Py:   s.count("a")
来源：http://umg.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://wqb.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://zmg.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://nog.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vmv.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://gjz.zhijiandao.cn

Ruby: s.count("a")
来源：http://kqj.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://pnv.yanxiufei.cn

[E13] 逐字符遍历
来源：http://jhl.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://xbc.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mdu.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bnv.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://olc.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rec.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nsc.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hdw.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ojn.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://iqx.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wkl.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dop.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qki.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vqk.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rnp.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://caq.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xas.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tnb.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://kxi.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qvb.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dxc.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mfi.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bkp.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uwy.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oeu.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lzi.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qpc.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://vbz.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://wwd.9152youxi.cn

PHP:  number_format(1234567);
来源：http://ccg.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://szr.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://smf.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://czc.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wms.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kmz.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://lry.uphjek.com

[E17] 首字母大写
来源：http://ijl.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gvs.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jtf.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogm.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gle.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://voe.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mqv.316326.xyz

Ruby: s.capitalize
来源：http://bvr.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yfr.yj20258.top

[E18] 模板占位符替换
来源：http://ddq.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lps.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kuv.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fdp.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://exn.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hbn.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vib.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://osy.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ztq.andypj.xyz

[E19] 多行文本按行拆分
来源：http://hzi.tanke756.top

Py:   s.splitlines()
来源：http://fer.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cly.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://kcw.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://ery.uphjek.com

Java: s.lines().toList()
来源：http://cyv.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://dbm.mhx1999.top

Ruby: s.lines
来源：http://wli.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://tal.yonumen.top

[E20] 判断字符串是否为空
来源：http://vyo.ctjpmb.com

Py:   if not s:
来源：http://thj.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://twh.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zrb.sxryk.cn

TS:   if (s === "") {}
来源：http://dlv.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://sud.zdbjq.cn

Go:   if s == "" {}
来源：http://oqj.xuetiantiany.cn

Ruby: if s.empty?
来源：http://pqw.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qru.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://yzv.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hnx.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mfs.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cmj.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pic.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qfg.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://cev.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tvw.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kdp.cashguo.top

[E22] 字节长度与字符长度
来源：http://nxx.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gwy.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cum.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://trt.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bij.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eaf.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rlt.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://mtq.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pzm.aizwys.cn

================================================================================
来源：http://awo.guannengcc.top

F. 文件与目录
来源：http://ukc.zhixingplan.top

================================================================================
来源：http://wpi.tarul.cn

[F01] 读取整个文件
来源：http://quq.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://imz.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://qsq.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gyi.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://szk.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sxk.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rhe.bjfxy.top

Ruby: File.read("a.txt")
来源：http://ggg.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://wax.sweek.top

[F02] 逐行读取文件
来源：http://rxl.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://psb.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ymo.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aju.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tlp.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bdd.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://syl.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pxw.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nyo.sweek.top

[F03] 写入文件（覆盖）
来源：http://vyb.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uoc.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://irw.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frv.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsw.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwv.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tts.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://hok.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rnc.hywenlv.cn

[F04] 追加写入文件
来源：http://wiy.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bum.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://luf.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvf.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cbf.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hgq.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://afd.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ndd.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ynm.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://iqc.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://khk.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://tqn.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://ebd.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://ivg.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xqb.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ypb.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://rok.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://vip.birdmap.top

[F06] 删除文件
来源：http://buy.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://lbc.ydzc1.top

PHP:  unlink("a.txt");
来源：http://scs.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://imv.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://hgt.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bem.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://wff.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://lim.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://hfn.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://fot.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mmj.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eme.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://smq.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vub.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bsm.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://orj.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ffm.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rsk.9152youxi.cn

[F08] 遍历目录
来源：http://qvi.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dpy.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yvb.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://zgf.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://omg.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nve.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uxm.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://xhs.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://kfa.yueranfly.top

[F09] 获取文件大小
来源：http://onz.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://opw.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://sdp.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://roi.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://lis.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://dnj.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://myu.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://dpm.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://mia.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://xzg.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ohy.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sni.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ajb.fengsongda.top

TS:   path.extname("a.txt")
来源：http://ekl.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fgp.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rgp.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dhi.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wqi.bbcook.cn

[F11] 复制与移动文件
来源：http://ycm.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jfp.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ren.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tkc.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edd.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mna.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pig.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nje.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vkc.yuxming.cn

[F12] CSV 读写
来源：http://qll.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vqs.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ban.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pmr.c1oappe.top

TS:   // 同上
来源：http://lxe.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uik.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hzi.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zbm.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lua.yangfankeji.com

================================================================================
来源：http://tfi.cashguo.top

G. 面向对象
来源：http://jpf.9152youxi.cn

================================================================================
来源：http://awf.jinyuanbaomall.cn

[G01] 定义类
来源：http://sjk.uphjek.com

Py:   class User: pass
来源：http://nag.yuxming.cn

PHP:  class User {}
来源：http://dlt.wangshuangyany.cn

JS:   class User {}
来源：http://pyo.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://krx.316326.xyz

Java: class User {}
来源：http://dsy.yangfankeji.com

Go:   type User struct { Name string }
来源：http://osd.birdmap.top

Ruby: class User; end
来源：http://fgw.zhengqikj.top

C#:   class User {}
来源：http://xmv.shanyushiyangtech.top

[G02] 构造函数
来源：http://dsl.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://omt.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://gsd.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://aja.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://oer.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://tna.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qsa.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://kkf.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://kvr.fanxiaobao.xyz

[G03] 实例属性
来源：http://urv.zhiwuduotai.top

Py:   self.name = "x"
来源：http://blq.daxiang520.top

PHP:  public string $name = "x";
来源：http://dvm.haohaochexian.top

JS:   this.name = "x";
来源：http://vyh.ydzc1.top

TS:   name: string = "x";
来源：http://rne.ivvv.top

Java: private String name;
来源：http://pxh.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wzn.zhongyouzk.top

Ruby: @name = "x"
来源：http://xca.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://wum.daria6918.cn

[G04] 定义方法
来源：http://dxb.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://guy.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://uhj.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://xda.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://bju.vqdsnc.cn

Java: String greet() { return name; }
来源：http://zsf.snrcjt.cn


<!-- 参考信息 -->