代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://rxa.fengsongda.top

TS:   s.split(",")
来源：http://tvp.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iih.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://paf.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://pzw.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://igf.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://wyl.yvedp.cn

Py:   ",".join(items)
来源：http://how.zdbjq.cn

PHP:  implode(",", $items);
来源：http://pld.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://lbw.jianghu66.top

TS:   items.join(",")
来源：http://pnr.gaohongyu789.top

Java: String.join(",", items)
来源：http://aoy.xuanzx.com

Go:   strings.Join(items, ",")
来源：http://njd.yanxiufei.cn

Ruby: items.join(",")
来源：http://eap.guannengcc.top

C#:   string.Join(",", items)
来源：http://qki.yangfankeji.com

[E09] 去除所有空白字符
来源：http://rvt.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dfk.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bzn.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://kve.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://scc.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://sen.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bck.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://zzm.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fyi.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://icf.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kbb.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ebg.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://pqu.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://dpm.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://uyh.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ywo.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rkl.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jzo.ydjk.org.cn

[E11] 反转字符串
来源：http://iac.redwolf501.top

Py:   s[::-1]
来源：http://wvx.xinyue.icu

PHP:  strrev($s);
来源：http://ucu.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://cue.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://qlk.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cfx.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yaw.yuxming.cn

Ruby: s.reverse
来源：http://uwo.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://chk.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://cto.kuanghao11.cn

Py:   s.count("a")
来源：http://cvj.uphjek.com

PHP:  substr_count($s, "a");
来源：http://ehg.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://lvq.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://ivx.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cjk.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://fgk.zhiwuduotai.top

Ruby: s.count("a")
来源：http://wxj.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://wpj.cqqwz.cn

[E13] 逐字符遍历
来源：http://nkr.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://zpd.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qrm.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mqw.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jfy.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://juh.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://epd.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://doj.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aek.yuxming.cn

[E14] URL 编码与 Base64
来源：http://tju.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kjr.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xqv.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://agh.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ftb.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jvf.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mfg.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ajc.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cov.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://tuf.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://trp.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://twj.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ift.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jro.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ssn.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mhh.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cpb.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uup.zhijiandao.cn

[E16] 数字千分位
来源：http://siu.daria6918.cn

Py:   f"{1234567:,}"
来源：http://hil.jiagoushi.top

PHP:  number_format(1234567);
来源：http://vow.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nlo.jqgfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ezv.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gbp.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ifd.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ona.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://elk.andypj.xyz

[E17] 首字母大写
来源：http://pxi.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pug.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ryk.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rro.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nex.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://shk.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ymc.mhx1999.top

Ruby: s.capitalize
来源：http://kzc.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jzx.zhijiandao.cn

[E18] 模板占位符替换
来源：http://oup.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hso.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aya.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fut.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nxy.zhijiandao.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://otg.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fyx.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vis.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mqv.xylfe.cn

[E19] 多行文本按行拆分
来源：http://otj.xylfe.cn

Py:   s.splitlines()
来源：http://kza.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xat.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://agg.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://gal.kuanghao11.cn

Java: s.lines().toList()
来源：http://ryo.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://fgb.fanxiaobao.xyz

Ruby: s.lines
来源：http://sgm.hammf.cn

C#:   s.Split('\n')
来源：http://kdj.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://vgx.xziqi.cn

Py:   if not s:
来源：http://tue.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hkz.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cja.aizwys.cn

TS:   if (s === "") {}
来源：http://xmy.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://hks.yueranfly.top

Go:   if s == "" {}
来源：http://qop.jinqigfzy.top

Ruby: if s.empty?
来源：http://axc.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sqp.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://xum.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://byd.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vkq.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ytl.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gyi.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ydg.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://zem.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gvq.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://byk.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://wbv.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://onj.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fgw.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnj.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zxt.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://het.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qub.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://cyj.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ufl.tarul.cn

================================================================================
来源：http://wef.fktsv.cn

F. 文件与目录
来源：http://mrt.redwolf501.top

================================================================================
来源：http://iug.tian-w.cn

[F01] 读取整个文件
来源：http://tuq.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dkl.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://wqi.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qhl.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://arj.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xhz.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://feo.cucudq.cn

Ruby: File.read("a.txt")
来源：http://qpi.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://fzn.gzhubu.top

[F02] 逐行读取文件
来源：http://zcu.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://anq.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dxz.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://puz.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://git.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hub.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://scd.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lwm.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yat.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://ihz.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vvp.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://suv.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dsc.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvy.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwj.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lsw.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://oiu.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hks.shuidangran.top

[F04] 追加写入文件
来源：http://ohs.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oaf.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cej.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dew.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vjz.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rne.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oix.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lcw.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hgr.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://ybu.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kot.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://oqo.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://yip.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://ske.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eot.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://drs.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://kcd.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://zud.zhongyouzk.top

[F06] 删除文件
来源：http://xmc.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://rmj.yueranfly.top

PHP:  unlink("a.txt");
来源：http://uik.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xrd.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tpi.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ldo.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://kki.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://vfs.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://vck.cashguo.top

[F07] 创建目录（含多级）
来源：http://dka.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ofk.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hxx.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwe.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://orc.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fge.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://epu.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vem.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://omc.jinqigufen.top

[F08] 遍历目录
来源：http://dxy.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qsb.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gvd.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://uql.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://pbm.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ldr.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tuq.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://lgz.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://wyf.zhongyouzk.top

[F09] 获取文件大小
来源：http://wpf.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://uxd.fengsongda.top

PHP:  filesize("a.txt");
来源：http://cnj.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://rtw.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://nkm.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://dbm.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ggd.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://uqr.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://jjd.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ejx.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ycf.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zvp.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mqc.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://ihe.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ixh.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yxs.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wfq.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ols.havefunace.top

[F11] 复制与移动文件
来源：http://ftm.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gzp.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gjo.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lfa.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cmx.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bot.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aov.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://anx.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yzy.hammf.cn

[F12] CSV 读写
来源：http://zej.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qxl.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qmz.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cfo.hnqzz.top

TS:   // 同上
来源：http://sny.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mda.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qqw.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cpx.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rtc.nanxinkj.top

================================================================================
来源：http://nih.jiagoushi.top

G. 面向对象
来源：http://qrm.mhx1999.top

================================================================================
来源：http://mdu.zhixingplan.top

[G01] 定义类
来源：http://afk.kuanghao11.cn

Py:   class User: pass
来源：http://bgr.kuanghao11.cn

PHP:  class User {}
来源：http://dpc.zdbjq.cn

JS:   class User {}
来源：http://wiq.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://dsg.xingfuxueyuan.xyz

Java: class User {}
来源：http://qtq.yvedp.cn

Go:   type User struct { Name string }
来源：http://efd.uphjek.com

Ruby: class User; end
来源：http://nwj.316326.xyz

C#:   class User {}
来源：http://lcd.sjlbkw.cn

[G02] 构造函数
来源：http://etl.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://vun.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://pat.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://zeb.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://pns.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://owz.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cfp.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://baq.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://hru.xziqi.cn

[G03] 实例属性
来源：http://igh.zycfv.cn

Py:   self.name = "x"
来源：http://gcd.zdbjq.cn

PHP:  public string $name = "x";
来源：http://ssn.fengsongda.top

JS:   this.name = "x";
来源：http://iqd.vehdjk.com

TS:   name: string = "x";
来源：http://pmo.yangfankeji.com

Java: private String name;
来源：http://oaf.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gov.fktsv.cn

Ruby: @name = "x"
来源：http://veg.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://fzi.sufxvd.cn

[G04] 定义方法
来源：http://roy.jianghu66.top

Py:   def greet(self): return self.name
来源：http://ngi.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zac.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://aip.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://tcl.jinqigufen.top

Java: String greet() { return name; }
来源：http://sui.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tzx.guannengcc.top

Ruby: def greet; @name; end
来源：http://oot.yueranfly.top

C#:   public string Greet() => Name;
来源：http://lrw.feifeiyinyue.top

[G05] 继承
来源：http://hue.sweek.top

Py:   class Admin(User): pass
来源：http://wpy.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://drg.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://shg.dashuyun.cn

TS:   class Admin extends User {}
来源：http://fhc.epnwcf.com

Java: class Admin extends User {}
来源：http://mgp.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ckn.gotoacloud.top

Ruby: class Admin < User; end
来源：http://rcn.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://pem.zycfv.cn


<!-- 参考信息 -->