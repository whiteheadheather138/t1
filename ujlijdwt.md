代发 wailian999

[E06] 替换子串
来源：http://vgz.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tqh.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://yby.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cla.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://soi.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ncl.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kti.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kah.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://qnt.chenzaomai.com

[E07] 按分隔符拆分
来源：http://nuw.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sic.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wfw.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ozz.gzhubu.top

TS:   s.split(",")
来源：http://uen.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://tgb.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://viq.sweek.top

Ruby: s.split(",");  s.split
来源：http://yir.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://idq.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://nef.haohaochexian.top

Py:   ",".join(items)
来源：http://faf.jinqigufen.top

PHP:  implode(",", $items);
来源：http://sue.xziqi.cn

JS:   items.join(",")
来源：http://bol.feifeiyinyue.top

TS:   items.join(",")
来源：http://fpw.yangfankeji.com

Java: String.join(",", items)
来源：http://mip.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://fav.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://tpb.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://pcr.gotoacloud.top

[E09] 去除所有空白字符
来源：http://mtc.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zei.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://avy.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://ffx.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://ukf.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://zut.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bip.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ezq.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eoz.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://yrj.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ukv.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hmh.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://xxv.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://xij.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://tpt.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rfo.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://edy.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kpl.yuxming.cn

[E11] 反转字符串
来源：http://wlx.zhongyouzk.top

Py:   s[::-1]
来源：http://xfy.bjfxy.top

PHP:  strrev($s);
来源：http://lip.sweek.top

JS:   [...s].reverse().join("")
来源：http://ekr.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://wvf.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xxb.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://cma.zhengqikj.top

Ruby: s.reverse
来源：http://lfu.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://chu.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://egt.hywenlv.cn

Py:   s.count("a")
来源：http://pli.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://scc.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://wqb.gzhubu.top

TS:   s.split("a").length - 1
来源：http://apb.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ogz.hammf.cn

Go:   strings.Count(s, "a")
来源：http://icb.chenlongwang.top

Ruby: s.count("a")
来源：http://ywd.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://yug.zhengqikj.top

[E13] 逐字符遍历
来源：http://set.yj202588.top

Py:   for ch in s: print(ch)
来源：http://lev.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tis.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uvy.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zpt.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qug.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://buv.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eep.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rjs.yfazqb.com

[E14] URL 编码与 Base64
来源：http://clk.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wnb.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jef.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jwd.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rts.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qoq.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gwq.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://his.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dfl.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://dfk.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zea.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ioy.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mvx.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tgm.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ltj.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bxa.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://igg.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jde.redwolf501.top

[E16] 数字千分位
来源：http://ehj.epnwcf.com

Py:   f"{1234567:,}"
来源：http://jdl.ppjwa.cn

PHP:  number_format(1234567);
来源：http://zbf.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gzy.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zoa.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jap.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qxu.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tlx.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://pof.hywenlv.cn

[E17] 首字母大写
来源：http://cty.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ihj.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://edn.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://erc.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://crh.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ftb.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wgw.cucudq.cn

Ruby: s.capitalize
来源：http://jcl.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ppk.mhx1999.top

[E18] 模板占位符替换
来源：http://tpm.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://psj.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bpd.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ikb.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rjg.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pbl.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sjm.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pwc.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yvk.meibo888.top

[E19] 多行文本按行拆分
来源：http://iyi.epnwcf.com

Py:   s.splitlines()
来源：http://rkn.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rnw.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://rhq.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://gvf.pycfn.com

Java: s.lines().toList()
来源：http://jls.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://hdk.yongpay.top

Ruby: s.lines
来源：http://atz.guowangkeji.top

C#:   s.Split('\n')
来源：http://idj.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://bht.redwolf501.top

Py:   if not s:
来源：http://okt.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qta.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ihx.bbcook.cn

TS:   if (s === "") {}
来源：http://csb.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://nhe.havefunace.top

Go:   if s == "" {}
来源：http://cqa.jyoumei.cn

Ruby: if s.empty?
来源：http://gef.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://znu.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://ksp.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yko.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dcj.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eaz.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ebi.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hvc.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://dvu.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://olx.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lyx.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://gfq.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txu.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mnx.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iba.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwf.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bwq.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hkz.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://qhf.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lzu.guannengcc.top

================================================================================
来源：http://qda.yfazqb.com

F. 文件与目录
来源：http://xee.jinghuilouyu.cn

================================================================================
来源：http://eyx.xziqi.cn

[F01] 读取整个文件
来源：http://uqf.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mdl.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://toe.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ins.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zse.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mtk.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hwq.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://hbr.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://abs.yvedp.cn

[F02] 逐行读取文件
来源：http://zxg.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tqj.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lib.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lni.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vic.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgw.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fml.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aof.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jmg.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://jkp.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fus.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://spx.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhp.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zdc.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://idm.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nul.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://mxs.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ios.hammf.cn

[F04] 追加写入文件
来源：http://phu.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ogl.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://asx.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://foo.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qke.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://irw.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pgy.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uqf.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rwe.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://qfk.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dlr.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://img.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://nnx.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://bss.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://hxl.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tjz.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://hhq.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://tbe.chenzaomai.com

[F06] 删除文件
来源：http://tyt.tian-w.cn

Py:   os.remove("a.txt")
来源：http://drd.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://agk.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://ltt.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xhw.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fkr.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://trz.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://mcx.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://mrl.yj20258.top

[F07] 创建目录（含多级）
来源：http://gqu.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jmp.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://utc.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yjx.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xjn.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jrt.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dub.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yxe.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yuj.cdnleiting.top

[F08] 遍历目录
来源：http://knz.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qkg.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://egz.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://bwi.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://acs.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xpv.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oif.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://kra.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://nks.hnxiangtu.top

[F09] 获取文件大小
来源：http://hdk.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://gfg.yueranfly.top

PHP:  filesize("a.txt");
来源：http://hpc.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://rlh.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://lsh.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ezm.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vvy.yj20258888.top

Ruby: File.size("a.txt")
来源：http://xem.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://sur.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://olf.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wuk.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rbi.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://soo.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://cuu.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eas.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ins.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sem.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://alj.ppjwa.cn

[F11] 复制与移动文件
来源：http://qkj.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wbk.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yzt.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hox.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gvp.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nho.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rrq.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gkr.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kbb.hcnkem.com

[F12] CSV 读写
来源：http://hyf.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ghw.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ozf.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cuv.jinyuanbaomall.cn

TS:   // 同上
来源：http://klp.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://amo.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ckk.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gez.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://opd.yj202588.top

================================================================================
来源：http://otn.cucudq.cn

G. 面向对象
来源：http://xui.zhijiandao.cn

================================================================================
来源：http://faf.shzxlz.cn

[G01] 定义类
来源：http://eof.redwolf501.top

Py:   class User: pass
来源：http://jrz.sxryk.cn

PHP:  class User {}
来源：http://qpo.chenlongwang.top

JS:   class User {}
来源：http://ary.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://lpr.jinyuanbaomall.cn

Java: class User {}
来源：http://etv.shuidangran.top

Go:   type User struct { Name string }
来源：http://xwy.hongshengwenyu.top

Ruby: class User; end
来源：http://xvg.ctjpmb.com

C#:   class User {}
来源：http://tyu.jlsjyb.cn

[G02] 构造函数
来源：http://joe.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://vpp.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://bjm.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://ish.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://aae.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://cpy.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bcq.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://fuj.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://pcv.hysaishi.cn

[G03] 实例属性
来源：http://kqt.zhiwuduotai.top

Py:   self.name = "x"
来源：http://tgw.hysaishi.cn

PHP:  public string $name = "x";
来源：http://wxh.52xcode.cn

JS:   this.name = "x";
来源：http://tzh.daxiang520.top

TS:   name: string = "x";
来源：http://dkt.snrcjt.cn

Java: private String name;
来源：http://lvf.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cen.feifeiyinyue.top

Ruby: @name = "x"
来源：http://ott.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://jeh.yj202588.top

[G04] 定义方法
来源：http://qjy.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://uga.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sfe.pycfn.com

JS:   greet() { return this.name; }
来源：http://qng.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://sgj.gaohongyu789.top

Java: String greet() { return name; }
来源：http://ndd.vehdjk.com


<!-- 参考信息 -->