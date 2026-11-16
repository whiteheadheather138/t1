代发 wailian999

[E06] 替换子串
来源：http://lsa.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fjb.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://lwu.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iln.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://xca.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://you.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yoa.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xea.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://rer.ctjpmb.com

[E07] 按分隔符拆分
来源：http://uzy.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wmw.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tmo.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mno.vehdjk.com

TS:   s.split(",")
来源：http://uwo.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://nvf.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lgj.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://rir.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iji.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://puu.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://glu.jinqigufen.top

PHP:  implode(",", $items);
来源：http://cle.cqqwz.cn

JS:   items.join(",")
来源：http://qdl.ybcxt.top

TS:   items.join(",")
来源：http://jjk.fktsv.cn

Java: String.join(",", items)
来源：http://gdk.birdmap.top

Go:   strings.Join(items, ",")
来源：http://ine.guowangkeji.top

Ruby: items.join(",")
来源：http://vzx.jiagoushi.top

C#:   string.Join(",", items)
来源：http://ylh.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://wlm.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eng.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hnd.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://cad.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://bmx.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://pqy.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ovu.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://oya.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ynx.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://hfx.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yyd.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yuj.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://tjz.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://rpw.yongpay.top

Java: String.format("%03d", 7)
来源：http://vid.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nqg.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aua.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pjk.tarul.cn

[E11] 反转字符串
来源：http://usv.hammf.cn

Py:   s[::-1]
来源：http://ygt.dianchejie.cn

PHP:  strrev($s);
来源：http://llh.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://waf.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://joh.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tab.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wit.gotoacloud.top

Ruby: s.reverse
来源：http://ipw.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://lyp.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://ybl.yueranfly.top

Py:   s.count("a")
来源：http://adq.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://esb.xziqi.cn

JS:   s.split("a").length - 1
来源：http://ohr.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://qah.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zqs.cashguo.top

Go:   strings.Count(s, "a")
来源：http://ntk.yj20258.top

Ruby: s.count("a")
来源：http://jjz.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://dra.ctjpmb.com

[E13] 逐字符遍历
来源：http://xtx.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://ijl.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nka.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jym.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hlw.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nuo.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yuw.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ocr.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yjk.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://ljt.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ddp.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hdj.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://znu.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vlo.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kte.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://clf.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wuf.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zbt.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://rlx.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ory.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://clw.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://svu.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nmw.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyf.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xnh.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jdw.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://knk.xinyue.icu

[E16] 数字千分位
来源：http://hzm.redwolf501.top

Py:   f"{1234567:,}"
来源：http://vsk.yj202588.top

PHP:  number_format(1234567);
来源：http://kmy.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bxu.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wrh.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tba.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xcj.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vuk.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://lsb.cucudq.cn

[E17] 首字母大写
来源：http://pjw.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xeq.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tvw.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yuz.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzc.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fms.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://alu.yuanzhike.top

Ruby: s.capitalize
来源：http://dtx.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://znd.chenlongwang.top

[E18] 模板占位符替换
来源：http://abe.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vju.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bwo.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cqv.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wzr.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fwt.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jdp.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nyd.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dvg.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://beo.daxiang520.top

Py:   s.splitlines()
来源：http://sfy.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vpl.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://sdt.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://zbn.xinyue.icu

Java: s.lines().toList()
来源：http://uuz.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://ylu.uphjek.com

Ruby: s.lines
来源：http://lbp.andypj.xyz

C#:   s.Split('\n')
来源：http://hfr.xinyue.icu

[E20] 判断字符串是否为空
来源：http://kvy.yfazqb.com

Py:   if not s:
来源：http://ubn.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://psv.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ftx.shuidangran.top

TS:   if (s === "") {}
来源：http://xal.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://xln.uphjek.com

Go:   if s == "" {}
来源：http://nvi.sysykeji.top

Ruby: if s.empty?
来源：http://iyx.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://edl.jiagoushi.top

[E21] 超长截断加省略号
来源：http://ihu.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vtq.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://frb.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kor.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axe.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bct.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://quh.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mrf.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xvt.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://nrt.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://exg.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://twl.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uae.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dzj.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://knl.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ruv.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://zgp.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tnn.316326.xyz

================================================================================
来源：http://hew.bjfxy.top

F. 文件与目录
来源：http://afq.xuanzx.com

================================================================================
来源：http://pzy.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://vxw.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lvd.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://gcp.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://epv.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://znt.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pab.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mep.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://jmf.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://pbk.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://dzc.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lmp.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yny.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://byp.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihj.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dls.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egl.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wgz.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ufz.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://qrl.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tpq.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://piv.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://omo.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfx.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ico.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xpu.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://dss.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwh.chenzaomai.com

[F04] 追加写入文件
来源：http://mfj.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jes.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yyt.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vzo.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsl.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kpz.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xup.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nbx.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pjb.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://zgk.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kha.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://nni.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://pnd.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://hkc.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://prz.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hmd.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://hlt.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://ixu.jinghuilouyu.cn

[F06] 删除文件
来源：http://tdq.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://ngv.iojbl.cn

PHP:  unlink("a.txt");
来源：http://nrn.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://miy.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://jby.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rsm.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://zng.ivvv.top

Ruby: File.delete("a.txt")
来源：http://lqc.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://sjb.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://pft.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jqp.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://epx.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgp.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxq.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fjn.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lyp.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uzz.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mjy.yueranfly.top

[F08] 遍历目录
来源：http://jrx.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://stb.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wkj.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://fub.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://ciu.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ucu.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nux.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://uuh.guowangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://off.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://rlw.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://zry.sysykeji.top

PHP:  filesize("a.txt");
来源：http://zvy.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://njr.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://rls.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://cin.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://als.meibo888.top

Ruby: File.size("a.txt")
来源：http://zjw.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://ogp.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://rae.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hso.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eao.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://swe.havefunace.top

TS:   path.extname("a.txt")
来源：http://fvy.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ajv.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zss.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qqz.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wwq.xylfe.cn

[F11] 复制与移动文件
来源：http://qrr.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bsn.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uss.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zzp.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ara.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ixu.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kgc.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ogi.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hyy.fzhhl.top

[F12] CSV 读写
来源：http://ili.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://okj.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dxf.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dza.cashguo.top

TS:   // 同上
来源：http://mqs.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://njs.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nfa.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mvi.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://aqm.tarul.cn

================================================================================
来源：http://srp.shuidangran.top

G. 面向对象
来源：http://zrs.jianghu66.top

================================================================================
来源：http://vcc.gzhubu.top

[G01] 定义类
来源：http://dol.ehwqpu.com

Py:   class User: pass
来源：http://gmp.fanxiaobao.xyz

PHP:  class User {}
来源：http://zmx.cashguo.top

JS:   class User {}
来源：http://bwf.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://kqt.fengsongda.top

Java: class User {}
来源：http://aro.fzhhl.top

Go:   type User struct { Name string }
来源：http://euc.bjfxy.top

Ruby: class User; end
来源：http://hxn.zdbjq.cn

C#:   class User {}
来源：http://jgt.feifeiyinyue.top

[G02] 构造函数
来源：http://gvm.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://gkt.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://qin.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://utq.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://tff.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://zmv.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jmi.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://xmh.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://ply.yangfankeji.com

[G03] 实例属性
来源：http://pex.vehdjk.com

Py:   self.name = "x"
来源：http://nup.smart0.xyz

PHP:  public string $name = "x";
来源：http://sya.tanke756.top

JS:   this.name = "x";
来源：http://feu.bjfxy.top

TS:   name: string = "x";
来源：http://olj.havefunace.top

Java: private String name;
来源：http://bgk.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mhu.zycfv.cn

Ruby: @name = "x"
来源：http://fqt.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://tho.jiagoushi.top

[G04] 定义方法
来源：http://vro.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://rax.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tcc.yj20258.top

JS:   greet() { return this.name; }
来源：http://tcr.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://xyl.gzhubu.top

Java: String greet() { return name; }
来源：http://dfo.fehbvm.com


<!-- 参考信息 -->