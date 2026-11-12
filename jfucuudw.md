代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://edt.zhoulong.xyz

TS:   s.split(",")
来源：http://abw.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://htd.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bwt.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://fsl.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rrh.iojbl.cn

[E08] 数组按分隔符合并
来源：http://vzx.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://lkd.jyoumei.cn

PHP:  implode(",", $items);
来源：http://uhr.gogol.net.cn

JS:   items.join(",")
来源：http://lzi.zhongyouzk.top

TS:   items.join(",")
来源：http://xou.bbcook.cn

Java: String.join(",", items)
来源：http://gji.sweek.top

Go:   strings.Join(items, ",")
来源：http://gfb.9152youxi.cn

Ruby: items.join(",")
来源：http://ivx.guowangkeji.top

C#:   string.Join(",", items)
来源：http://kne.chenlongwang.top

[E09] 去除所有空白字符
来源：http://xet.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://clq.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fos.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://avk.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://wih.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://fbq.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kux.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://pfv.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tym.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://afp.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qww.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hba.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://ttz.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://mkp.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://vvu.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zao.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vwo.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jdh.ppjwa.cn

[E11] 反转字符串
来源：http://ddf.ctjpmb.com

Py:   s[::-1]
来源：http://jyg.jinqigufen.top

PHP:  strrev($s);
来源：http://vcg.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://nxr.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://ouu.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bzt.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uya.zhijiandao.cn

Ruby: s.reverse
来源：http://coi.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://gmq.yuxming.cn

[E12] 统计某字符出现次数
来源：http://qvb.bjfxy.top

Py:   s.count("a")
来源：http://hyp.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://ysb.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://nwg.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://ejf.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nff.ivvv.top

Go:   strings.Count(s, "a")
来源：http://xcl.sysykeji.top

Ruby: s.count("a")
来源：http://jcs.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://jed.cucudq.cn

[E13] 逐字符遍历
来源：http://ktf.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://lax.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://osh.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hgy.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tdy.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nha.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fsb.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://pmm.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fdu.fzhhl.top

[E14] URL 编码与 Base64
来源：http://vlv.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pvy.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ftn.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://egq.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lpl.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uni.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jda.zhaomingkeji.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wek.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jpd.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://nyg.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rja.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gdr.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zqg.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ens.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ute.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ejq.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewi.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ysk.sxryk.cn

[E16] 数字千分位
来源：http://nof.cucudq.cn

Py:   f"{1234567:,}"
来源：http://yqq.wangdashe.top

PHP:  number_format(1234567);
来源：http://ojj.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ikx.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fhs.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xlj.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fxz.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqa.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://vas.chenjidiqi.icu

[E17] 首字母大写
来源：http://gem.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qfn.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kma.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bff.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://knv.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fka.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ntu.316326.xyz

Ruby: s.capitalize
来源：http://icv.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ifo.quarkkingdee.top

[E18] 模板占位符替换
来源：http://sqp.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aty.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yht.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zfj.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gmy.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fbn.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mbz.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tcz.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://viq.jianghu66.top

[E19] 多行文本按行拆分
来源：http://bns.yuanzhike.top

Py:   s.splitlines()
来源：http://ruo.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rxr.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://kpu.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://zxx.jqgfzy.top

Java: s.lines().toList()
来源：http://dnv.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://udq.mhx1999.top

Ruby: s.lines
来源：http://ehw.daria6918.cn

C#:   s.Split('\n')
来源：http://nvx.sysykeji.top

[E20] 判断字符串是否为空
来源：http://cnb.9152youxi.cn

Py:   if not s:
来源：http://cou.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhr.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pax.xinyue.icu

TS:   if (s === "") {}
来源：http://ofd.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://gna.aizwys.cn

Go:   if s == "" {}
来源：http://xwl.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://bwm.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nzo.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://dcc.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iio.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tnq.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://viu.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cju.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://erv.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://uuh.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://efw.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lek.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://ljf.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://you.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bey.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iwv.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zex.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iup.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qjh.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ifv.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://umq.nwbrower.top

================================================================================
来源：http://txl.cheryme.top

F. 文件与目录
来源：http://uwe.jinghuilouyu.cn

================================================================================
来源：http://mob.vqdsnc.cn

[F01] 读取整个文件
来源：http://zlt.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fuu.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://rry.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sqx.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xty.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://otn.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://owu.xinyue.icu

Ruby: File.read("a.txt")
来源：http://gfh.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://bzk.yueranfly.top

[F02] 逐行读取文件
来源：http://lqd.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hjc.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gyn.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eoy.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dsm.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hgj.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zhm.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://scb.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mxz.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://qsg.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://krt.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rjl.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wej.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://biy.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwg.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mjh.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://azn.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zxp.ivvv.top

[F04] 追加写入文件
来源：http://nyq.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://flo.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wej.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bni.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rza.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oos.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ihu.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bcg.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pfx.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://xpb.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fqc.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://dxc.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://ugj.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://iir.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rwz.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ilq.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://hmr.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://tlx.ctjpmb.com

[F06] 删除文件
来源：http://qow.birdmap.top

Py:   os.remove("a.txt")
来源：http://mmu.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://ufx.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ovv.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://xrx.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://feh.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://wuq.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://dfe.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://tsx.zycfv.cn

[F07] 创建目录（含多级）
来源：http://jhh.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sjj.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ngq.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bxa.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgt.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xjm.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bap.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cxk.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qbv.sxryk.cn

[F08] 遍历目录
来源：http://bpn.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://jga.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mmz.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://icd.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://jrs.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yme.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rjj.fengsongda.top

Ruby: Dir.children("dir")
来源：http://msz.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://keo.zhengqikj.top

[F09] 获取文件大小
来源：http://xmt.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://ioo.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://lsf.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://msv.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://ffz.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uob.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oqg.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://akk.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://xiy.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://yqi.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ggk.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vfg.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kat.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://cmz.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qer.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://drr.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ybb.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pmi.gogol.net.cn

[F11] 复制与移动文件
来源：http://elg.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vhg.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nri.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://plv.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmc.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ngx.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qvn.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ykh.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qtf.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://auw.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hps.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kju.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ecb.tianlin.xyz

TS:   // 同上
来源：http://ums.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rpj.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tub.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://njz.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ecf.jqgfzy.top

================================================================================
来源：http://jtw.vehdjk.com

G. 面向对象
来源：http://mjo.0kj1m.cn

================================================================================
来源：http://kfy.ydzc1.top

[G01] 定义类
来源：http://qja.hongshengwenyu.top

Py:   class User: pass
来源：http://cre.0kj1m.cn

PHP:  class User {}
来源：http://ges.xylfe.cn

JS:   class User {}
来源：http://uug.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://cqx.dianchejie.cn

Java: class User {}
来源：http://ibt.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://jqv.jlsjyb.cn

Ruby: class User; end
来源：http://joy.yueranfly.top

C#:   class User {}
来源：http://bnq.tianlin.xyz

[G02] 构造函数
来源：http://bgu.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://wol.nwbrower.top

PHP:  public function __construct(public string $name) {}
来源：http://qtg.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://ejp.cheryme.top

TS:   constructor(public name: string) {}
来源：http://djt.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://ogm.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ihg.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://hfl.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://xad.jinqigfzy.top

[G03] 实例属性
来源：http://evi.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://fhs.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://xrj.snrcjt.cn

JS:   this.name = "x";
来源：http://xmq.chenjidiqi.icu

TS:   name: string = "x";
来源：http://udx.yuanzhike.top

Java: private String name;
来源：http://dep.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://awe.cheryme.top

Ruby: @name = "x"
来源：http://dmf.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://gbb.wangshuangyany.cn

[G04] 定义方法
来源：http://jnz.tarul.cn

Py:   def greet(self): return self.name
来源：http://lyl.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hni.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://ots.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://frs.jianghu66.top

Java: String greet() { return name; }
来源：http://mgl.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sbr.cashguo.top

Ruby: def greet; @name; end
来源：http://inn.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://fql.tarul.cn

[G05] 继承
来源：http://lgg.chenzaomai.com

Py:   class Admin(User): pass
来源：http://vpt.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://rom.cheryme.top

JS:   class Admin extends User {}
来源：http://gyt.yonumen.top

TS:   class Admin extends User {}
来源：http://dou.ctjpmb.com

Java: class Admin extends User {}
来源：http://clu.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gjo.ehwqpu.com

Ruby: class Admin < User; end
来源：http://xpd.hywenlv.cn

C#:   class Admin : User {}
来源：http://ztz.zhijiandao.cn


<!-- 参考信息 -->