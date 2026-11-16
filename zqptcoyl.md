代发 wailian999

C#:   s.Replace("a", "b")
来源：http://lda.havefunace.top

[E07] 按分隔符拆分
来源：http://yuf.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uwc.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hjp.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kri.guannengcc.top

TS:   s.split(",")
来源：http://cai.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://vfx.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://soc.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://ygt.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cjq.tanke756.top

[E08] 数组按分隔符合并
来源：http://tzc.redwolf501.top

Py:   ",".join(items)
来源：http://top.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://uum.uphjek.com

JS:   items.join(",")
来源：http://znq.vehdjk.com

TS:   items.join(",")
来源：http://wdm.ppjwa.cn

Java: String.join(",", items)
来源：http://nkt.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://jur.sjlbkw.cn

Ruby: items.join(",")
来源：http://aie.cheryme.top

C#:   string.Join(",", items)
来源：http://zlf.chenlongwang.top

[E09] 去除所有空白字符
来源：http://eqq.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ami.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qzp.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://qif.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://hdq.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://cel.9152youxi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://raq.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://bus.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ibs.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://bkn.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wvt.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iwn.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://mrk.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://jok.sweek.top

Java: String.format("%03d", 7)
来源：http://pys.guannengcc.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ndl.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hrx.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://olu.birdmap.top

[E11] 反转字符串
来源：http://rnj.guowangkeji.top

Py:   s[::-1]
来源：http://lsj.hcnkem.com

PHP:  strrev($s);
来源：http://nxa.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://gwn.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://jiw.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xsk.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rzv.cashguo.top

Ruby: s.reverse
来源：http://bjb.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lfq.xinyue.icu

[E12] 统计某字符出现次数
来源：http://hsk.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://mwb.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://nbr.tarul.cn

JS:   s.split("a").length - 1
来源：http://nsg.yueranfly.top

TS:   s.split("a").length - 1
来源：http://gup.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qus.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://ngr.jinqigufen.top

Ruby: s.count("a")
来源：http://gfj.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://nyk.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://imy.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://dze.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wec.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mrq.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mvv.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xbx.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yeq.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://trs.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qpz.fktsv.cn

[E14] URL 编码与 Base64
来源：http://teo.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cmw.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jcz.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://byb.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://msl.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zzd.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mbi.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mes.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sww.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://kzf.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kcq.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://agp.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ioe.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ukb.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pyz.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ugc.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://giz.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bli.fanxiaobao.xyz

[E16] 数字千分位
来源：http://qhi.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://smx.snrcjt.cn

PHP:  number_format(1234567);
来源：http://hkm.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fhh.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ymh.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fnw.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xdd.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uwv.meibo888.top

C#:   1234567.ToString("N0")
来源：http://ygc.cqqwz.cn

[E17] 首字母大写
来源：http://qfq.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hlr.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ptx.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dtm.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mbr.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jim.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cmb.kuanghao11.cn

Ruby: s.capitalize
来源：http://wip.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kvd.cdnleiting.top

[E18] 模板占位符替换
来源：http://akh.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nnx.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://awr.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mvt.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cqr.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bdx.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zob.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ept.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nqu.yvedp.cn

[E19] 多行文本按行拆分
来源：http://pec.fehbvm.com

Py:   s.splitlines()
来源：http://xty.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://thf.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://mdc.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://jbw.aizwys.cn

Java: s.lines().toList()
来源：http://maq.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://uxs.guannengcc.top

Ruby: s.lines
来源：http://nfo.zhijiandao.cn

C#:   s.Split('\n')
来源：http://cvi.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://ysb.hnqzz.top

Py:   if not s:
来源：http://bma.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wbw.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fpe.fzhhl.top

TS:   if (s === "") {}
来源：http://eli.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://hhp.chenjidiqi.icu

Go:   if s == "" {}
来源：http://tux.yongpay.top

Ruby: if s.empty?
来源：http://ekg.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wzo.chenlongwang.top

[E21] 超长截断加省略号
来源：http://ljb.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://duk.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jbx.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tqw.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsp.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vuj.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://ake.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jav.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ykq.fzhhl.top

[E22] 字节长度与字符长度
来源：http://jyg.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wag.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hms.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://usc.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yfe.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uyi.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uly.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://cfd.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qoy.andypj.xyz

================================================================================
来源：http://wyb.yvedp.cn

F. 文件与目录
来源：http://odj.jyoumei.cn

================================================================================
来源：http://lpp.chenlongwang.top

[F01] 读取整个文件
来源：http://hiv.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jcc.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://gqg.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iso.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://scx.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xhh.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pts.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://ygj.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://sfz.gzhubu.top

[F02] 逐行读取文件
来源：http://lof.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zrz.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ixu.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uvq.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iju.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://woe.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kjh.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sol.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pih.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://yzg.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://haz.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ybp.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksm.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lhy.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fsm.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmx.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://kpp.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://szk.nanxinkj.top

[F04] 追加写入文件
来源：http://ufw.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nui.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bvc.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fji.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrv.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cwa.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fuq.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yom.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qcd.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://eco.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blw.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://jxg.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://tci.sweek.top

TS:   fs.existsSync("a.txt")
来源：http://ooq.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://spe.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qpy.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://bhz.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://nzj.hnqzz.top

[F06] 删除文件
来源：http://poz.shuidangran.top

Py:   os.remove("a.txt")
来源：http://bzn.sweek.top

PHP:  unlink("a.txt");
来源：http://kqj.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://tpx.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://otr.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ybw.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://mfa.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://bvq.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://cmw.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://moa.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rjb.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hca.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zsk.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wer.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iux.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wtz.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hep.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jon.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://qvw.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uzz.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mhm.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://zvh.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://wvk.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sfo.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zdi.daria6918.cn

Ruby: Dir.children("dir")
来源：http://dlg.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://rfu.fengsongda.top

[F09] 获取文件大小
来源：http://nvo.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://xsc.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://tpe.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://bpq.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://djv.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://smm.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zee.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://zbs.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://acc.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://raw.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mne.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qmu.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xxv.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://lcv.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mgt.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ylp.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vpl.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://phc.fengsongda.top

[F11] 复制与移动文件
来源：http://yno.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ndu.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fbg.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lim.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://obp.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lnq.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://scn.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ifq.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gvz.tarul.cn

[F12] CSV 读写
来源：http://aps.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qij.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fyr.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nhv.ybcxt.top

TS:   // 同上
来源：http://cnu.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gkh.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://psz.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://spu.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vwo.uphjek.com

================================================================================
来源：http://rqk.tarul.cn

G. 面向对象
来源：http://zfg.meibo888.top

================================================================================
来源：http://pkt.hnqzz.top

[G01] 定义类
来源：http://qje.jinqigufen.top

Py:   class User: pass
来源：http://eda.hcnkem.com

PHP:  class User {}
来源：http://qpn.pengpengdd.cyou

JS:   class User {}
来源：http://bxm.yj20258.top

TS:   class User { name: string = ""; }
来源：http://onx.fengsongda.top

Java: class User {}
来源：http://mou.316326.xyz

Go:   type User struct { Name string }
来源：http://jlc.dianchejie.cn

Ruby: class User; end
来源：http://iab.zdbjq.cn

C#:   class User {}
来源：http://zrn.sxryk.cn

[G02] 构造函数
来源：http://iwr.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://jnw.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://exe.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://hhk.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://yve.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://cjl.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ugg.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://ejz.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://wyl.zhoulong.xyz

[G03] 实例属性
来源：http://kfc.0kj1m.cn

Py:   self.name = "x"
来源：http://ood.sysykeji.top

PHP:  public string $name = "x";
来源：http://tua.yanxiufei.cn

JS:   this.name = "x";
来源：http://tii.zhixingplan.top

TS:   name: string = "x";
来源：http://apf.nwbrower.top

Java: private String name;
来源：http://qwn.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yte.svipenyu.cn

Ruby: @name = "x"
来源：http://hgo.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://skp.mhx1999.top

[G04] 定义方法
来源：http://xub.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://kyc.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://crs.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://iol.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://omp.ppjwa.cn

Java: String greet() { return name; }
来源：http://dqi.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://shx.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://fjx.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://ihn.zdbjq.cn

[G05] 继承
来源：http://zhn.gotoacloud.top

Py:   class Admin(User): pass
来源：http://qak.tanke756.top

PHP:  class Admin extends User {}
来源：http://uef.cucudq.cn

JS:   class Admin extends User {}
来源：http://sib.tianlin.xyz

TS:   class Admin extends User {}
来源：http://qfv.hesvh.cn


<!-- 参考信息 -->