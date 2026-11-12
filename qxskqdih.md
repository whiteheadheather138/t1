代发 wailian999

C#:   s.Replace("a", "b")
来源：http://glp.pycfn.com

[E07] 按分隔符拆分
来源：http://yjw.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wdt.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://efj.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zdb.cqqwz.cn

TS:   s.split(",")
来源：http://ljr.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://efy.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fie.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://tnt.hywenlv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xtg.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://wby.nwbrower.top

Py:   ",".join(items)
来源：http://bhi.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://aox.sufxvd.cn

JS:   items.join(",")
来源：http://lbn.cqqwz.cn

TS:   items.join(",")
来源：http://gfv.nanxinkj.top

Java: String.join(",", items)
来源：http://dal.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://zrk.zdbjq.cn

Ruby: items.join(",")
来源：http://pwo.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://lde.andypj.xyz

[E09] 去除所有空白字符
来源：http://tqj.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ned.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yrw.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://gok.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://gpb.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://cgr.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mfw.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://qqd.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rku.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://zcm.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cjw.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rbs.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://etw.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://ujt.fzhhl.top

Java: String.format("%03d", 7)
来源：http://wvs.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ysg.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ags.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jik.daria6918.cn

[E11] 反转字符串
来源：http://gxb.sxryk.cn

Py:   s[::-1]
来源：http://eak.yonumen.top

PHP:  strrev($s);
来源：http://fxg.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://mlp.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://cwf.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vis.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oup.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://csp.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://ytw.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://qgk.hnxiangtu.top

Py:   s.count("a")
来源：http://fst.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://hfb.smart0.xyz

JS:   s.split("a").length - 1
来源：http://dpt.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://xlx.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fgl.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://hfx.52xcode.cn

Ruby: s.count("a")
来源：http://yay.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://pvp.wangdashe.top

[E13] 逐字符遍历
来源：http://bph.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://wbc.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ycb.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://tdn.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ggb.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lgz.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fqa.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dwp.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vqa.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://xay.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hdc.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ezv.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qjv.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mbe.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vft.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wsd.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oiv.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mjr.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://hmt.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kzb.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://teo.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tco.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://msw.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blb.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fre.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wzo.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pkd.iojbl.cn

[E16] 数字千分位
来源：http://wid.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://jrp.daxiang520.top

PHP:  number_format(1234567);
来源：http://gjl.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ckj.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pyr.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zqz.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzl.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mnh.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://wiu.fengsongda.top

[E17] 首字母大写
来源：http://qne.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rkb.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://dye.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://faw.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rvg.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qzj.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ozu.cashguo.top

Ruby: s.capitalize
来源：http://zst.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kjx.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://koy.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tmp.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ick.gaohongyu789.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fpl.xziqi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jpr.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qio.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jxx.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eyo.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://swm.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://gdu.sufxvd.cn

Py:   s.splitlines()
来源：http://ska.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aqz.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://kfr.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://jdf.zhixingplan.top

Java: s.lines().toList()
来源：http://ngu.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://wka.gzhubu.top

Ruby: s.lines
来源：http://xdc.jlsjyb.cn

C#:   s.Split('\n')
来源：http://prq.tanke756.top

[E20] 判断字符串是否为空
来源：http://nle.tanke756.top

Py:   if not s:
来源：http://jzu.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eqk.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zgf.zhoulong.xyz

TS:   if (s === "") {}
来源：http://zmp.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://zoj.zhongyouzk.top

Go:   if s == "" {}
来源：http://her.tanke756.top

Ruby: if s.empty?
来源：http://rnf.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uft.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://hmn.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ajq.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vem.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lyh.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xpz.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wsc.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://pnq.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eho.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rxn.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://vgc.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xul.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qrf.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://igg.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fuv.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iea.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pjh.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://sav.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pto.meibo888.top

================================================================================
来源：http://yag.chenjidiqi.icu

F. 文件与目录
来源：http://hjq.gzhubu.top

================================================================================
来源：http://fxo.iojbl.cn

[F01] 读取整个文件
来源：http://sbu.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aap.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://ukb.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bhi.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://epm.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pns.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ehz.chenzaomai.com

Ruby: File.read("a.txt")
来源：http://mvw.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://tmm.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://knr.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cvh.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://has.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tjr.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mge.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sic.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://htb.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://atd.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vjs.meibo888.top

[F03] 写入文件（覆盖）
来源：http://wbg.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wtp.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tcn.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lix.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iuu.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://clk.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://owg.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://mrl.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://efh.vqdsnc.cn

[F04] 追加写入文件
来源：http://tne.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gsy.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rqe.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gww.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgq.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sfu.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wel.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dpu.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nra.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://wyz.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jjs.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://ivd.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://swp.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://fio.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ugu.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sdv.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://iqn.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://ntx.feifeiyinyue.top

[F06] 删除文件
来源：http://rby.aizwys.cn

Py:   os.remove("a.txt")
来源：http://scn.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://wuh.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://sox.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hhm.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jhz.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://llw.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://tlt.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://awz.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://ekv.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hir.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dwy.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://muv.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vqv.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gji.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fsu.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gyw.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mxs.ybcxt.top

[F08] 遍历目录
来源：http://rfk.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cbm.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ykm.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://tpk.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://tep.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yam.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dqo.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://ffd.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://pag.gaohongyu789.top

[F09] 获取文件大小
来源：http://wqu.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://ctm.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://ioe.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://wwn.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://mcb.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://hew.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dla.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://azq.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://fct.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://qes.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oyv.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aww.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ivk.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://fkx.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bzi.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qri.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sel.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vto.uphjek.com

[F11] 复制与移动文件
来源：http://dxq.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://upj.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ool.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eqw.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zko.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://psk.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zeh.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xqx.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://clf.hesvh.cn

[F12] CSV 读写
来源：http://zav.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lkr.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xzg.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://shh.daxiang520.top

TS:   // 同上
来源：http://mqh.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qyn.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kuw.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gzk.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xlz.kuanghao11.cn

================================================================================
来源：http://phc.yanxiufei.cn

G. 面向对象
来源：http://dfz.yonumen.top

================================================================================
来源：http://aon.tian-w.cn

[G01] 定义类
来源：http://mgi.yj20258888.top

Py:   class User: pass
来源：http://ref.guowangkeji.top

PHP:  class User {}
来源：http://ofu.9152youxi.cn

JS:   class User {}
来源：http://zup.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://ooe.smart0.xyz

Java: class User {}
来源：http://vmg.xylfe.cn

Go:   type User struct { Name string }
来源：http://toy.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://osl.iojbl.cn

C#:   class User {}
来源：http://ijb.nanxuanxn.top

[G02] 构造函数
来源：http://qbj.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ufj.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://knp.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://jxg.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://dcn.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://fmq.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ana.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://dxp.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://fqb.fktsv.cn

[G03] 实例属性
来源：http://fhs.haohaochexian.top

Py:   self.name = "x"
来源：http://knc.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://ype.sxryk.cn

JS:   this.name = "x";
来源：http://zou.zdqjudy.top

TS:   name: string = "x";
来源：http://ykx.316326.xyz

Java: private String name;
来源：http://ykk.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mba.cashguo.top

Ruby: @name = "x"
来源：http://hzq.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://rpj.jlsjyb.cn

[G04] 定义方法
来源：http://lau.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://rwv.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gfl.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://xje.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://nef.sufxvd.cn

Java: String greet() { return name; }
来源：http://exi.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://noa.316326.xyz

Ruby: def greet; @name; end
来源：http://jfj.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://tjs.gotoacloud.top

[G05] 继承
来源：http://ixr.yuxming.cn

Py:   class Admin(User): pass
来源：http://fuz.uphjek.com

PHP:  class Admin extends User {}
来源：http://fyt.yj202588.top

JS:   class Admin extends User {}
来源：http://wjo.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://gof.mhx1999.top


<!-- 参考信息 -->