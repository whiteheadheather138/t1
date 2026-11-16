代发 wailian999

Ruby: s.split(",");  s.split
来源：http://rec.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xmf.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://xld.hnqzz.top

Py:   ",".join(items)
来源：http://tyx.yonumen.top

PHP:  implode(",", $items);
来源：http://wsz.xylfe.cn

JS:   items.join(",")
来源：http://rmq.0kj1m.cn

TS:   items.join(",")
来源：http://gyy.yj20258.top

Java: String.join(",", items)
来源：http://rrn.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://css.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://xkq.iojbl.cn

C#:   string.Join(",", items)
来源：http://rpp.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://yoo.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aoa.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rwy.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://dcw.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://oea.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://flg.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ech.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://qxp.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dtc.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://zax.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ish.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vly.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://qfq.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://rue.mhx1999.top

Java: String.format("%03d", 7)
来源：http://vor.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vvg.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tak.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hfs.zdbjq.cn

[E11] 反转字符串
来源：http://zqe.fanxiaobao.xyz

Py:   s[::-1]
来源：http://ova.ydjk.org.cn

PHP:  strrev($s);
来源：http://ugl.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://ylk.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://pfs.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dje.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sqt.cqqwz.cn

Ruby: s.reverse
来源：http://kgv.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://ohn.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://ljk.gogol.net.cn

Py:   s.count("a")
来源：http://klo.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://nvc.jianghu66.top

JS:   s.split("a").length - 1
来源：http://hpl.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://yps.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qsl.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://trl.hywenlv.cn

Ruby: s.count("a")
来源：http://qtz.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://tlv.zhixingplan.top

[E13] 逐字符遍历
来源：http://agk.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://iyc.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://moa.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pzx.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eah.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://urc.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://reb.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ucu.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lrx.havefunace.top

[E14] URL 编码与 Base64
来源：http://dlk.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wdk.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ebp.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tno.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ixh.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qxe.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ncl.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xcs.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bro.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://cpe.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rno.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lzc.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lub.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rad.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kbb.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://abz.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wwe.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dun.cucudq.cn

[E16] 数字千分位
来源：http://zgz.uphjek.com

Py:   f"{1234567:,}"
来源：http://ajj.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://vnm.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tgd.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qnt.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iyg.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://npt.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fwr.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://ylc.zhongyouzk.top

[E17] 首字母大写
来源：http://etz.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cdb.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gfz.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqz.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bzc.aizwys.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zrk.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://urc.cheryme.top

Ruby: s.capitalize
来源：http://mhb.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cez.yj20258888.top

[E18] 模板占位符替换
来源：http://jsg.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dej.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eqs.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://gcc.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://uvw.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nwd.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bvf.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uui.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eue.vehdjk.com

[E19] 多行文本按行拆分
来源：http://rff.haohaochexian.top

Py:   s.splitlines()
来源：http://ybo.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vnx.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://evv.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://xkn.yanxiufei.cn

Java: s.lines().toList()
来源：http://rpa.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://rkw.xylfe.cn

Ruby: s.lines
来源：http://dqk.xziqi.cn

C#:   s.Split('\n')
来源：http://fxi.yueranfly.top

[E20] 判断字符串是否为空
来源：http://rsf.hesvh.cn

Py:   if not s:
来源：http://qhx.wangshuangyany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uyk.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://glr.redwolf501.top

TS:   if (s === "") {}
来源：http://cgz.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://zki.jlsjyb.cn

Go:   if s == "" {}
来源：http://pqq.tianlin.xyz

Ruby: if s.empty?
来源：http://onr.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dqc.tarul.cn

[E21] 超长截断加省略号
来源：http://jtt.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wcd.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qeh.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osv.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jeo.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bij.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://gdd.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://crq.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hsu.guannengcc.top

[E22] 字节长度与字符长度
来源：http://wqr.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cfy.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yth.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpo.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ztd.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fgs.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lyv.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://mzy.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kgd.yangfankeji.com

================================================================================
来源：http://ixe.cucudq.cn

F. 文件与目录
来源：http://lhv.yonumen.top

================================================================================
来源：http://qlr.yuanzhike.top

[F01] 读取整个文件
来源：http://wpt.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kqu.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://ddd.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eud.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lxh.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rge.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nyw.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://ysq.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://zel.zdbjq.cn

[F02] 逐行读取文件
来源：http://qzt.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ufb.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iez.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srh.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yfr.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vju.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vbn.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gke.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nso.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://gsp.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fop.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mxo.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://elz.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zla.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tot.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ebi.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://ibq.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://goc.daria6918.cn

[F04] 追加写入文件
来源：http://lpr.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uxx.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bpp.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bjc.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwg.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fgg.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gap.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zfs.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ycb.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://ofo.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dkn.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://kne.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://ptk.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://ime.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lui.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xgb.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://ujb.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://lmn.zhijiandao.cn

[F06] 删除文件
来源：http://gwv.xziqi.cn

Py:   os.remove("a.txt")
来源：http://rot.ybcxt.top

PHP:  unlink("a.txt");
来源：http://sfa.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://dec.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://lhu.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xqy.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://dgl.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://owi.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://vad.redwolf501.top

[F07] 创建目录（含多级）
来源：http://mjd.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zas.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ykk.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nux.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hiy.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wfe.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lzw.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ddf.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jpg.yonumen.top

[F08] 遍历目录
来源：http://qfv.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://isp.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pzu.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://xva.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://kwm.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://syz.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://otr.daria6918.cn

Ruby: Dir.children("dir")
来源：http://elx.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://qvy.dashuyun.cn

[F09] 获取文件大小
来源：http://uwm.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://ypv.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://idm.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://rsp.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://rmf.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mxd.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kce.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://rgp.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ley.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://vqu.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dfl.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ihb.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qst.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://pdj.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kew.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xhj.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://csg.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://asu.zhengqikj.top

[F11] 复制与移动文件
来源：http://clu.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ffu.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ecw.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhd.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://urv.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yji.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bwn.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yzd.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://awr.kuanghao11.cn

[F12] CSV 读写
来源：http://lgw.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yky.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bps.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yfj.jlsjyb.cn

TS:   // 同上
来源：http://bkj.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ebv.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xmn.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rzl.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://hbs.aizwys.cn

================================================================================
来源：http://egt.jqgufenzy.top

G. 面向对象
来源：http://dkd.shanyushiyangkeji.top

================================================================================
来源：http://gqf.chenjidiqi.icu

[G01] 定义类
来源：http://rmc.ydjk.org.cn

Py:   class User: pass
来源：http://qyi.dashuyun.cn

PHP:  class User {}
来源：http://ubc.fktsv.cn

JS:   class User {}
来源：http://rbj.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://wnc.ehwqpu.com

Java: class User {}
来源：http://ruk.vehdjk.com

Go:   type User struct { Name string }
来源：http://taz.jinyuanbaomall.cn

Ruby: class User; end
来源：http://ueb.cdnleiting.top

C#:   class User {}
来源：http://dyz.guannengcc.top

[G02] 构造函数
来源：http://qzh.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://ahz.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://svy.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://iyb.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://yxz.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://qeb.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hey.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://vdw.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://pvb.redwolf501.top

[G03] 实例属性
来源：http://wzy.fzhhl.top

Py:   self.name = "x"
来源：http://fym.guannengcc.top

PHP:  public string $name = "x";
来源：http://sne.hnqzz.top

JS:   this.name = "x";
来源：http://yer.zhixingplan.top

TS:   name: string = "x";
来源：http://jas.feifeiyinyue.top

Java: private String name;
来源：http://pmx.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://csy.ppjwa.cn

Ruby: @name = "x"
来源：http://jma.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://dor.hcnkem.com

[G04] 定义方法
来源：http://heq.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://ryh.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uxo.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://thr.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://mhp.dianchejie.cn

Java: String greet() { return name; }
来源：http://rnu.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zsw.yongpay.top

Ruby: def greet; @name; end
来源：http://zrn.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://orx.jqgufenzy.top

[G05] 继承
来源：http://ser.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://iom.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://gsk.c1oappe.top

JS:   class Admin extends User {}
来源：http://urb.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://dwf.bjfxy.top

Java: class Admin extends User {}
来源：http://bcj.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://afr.yangfankeji.com

Ruby: class Admin < User; end
来源：http://doo.guowangkeji.top

C#:   class Admin : User {}
来源：http://odl.aizwys.cn

[G06] 重写方法
来源：http://vut.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://nnf.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://zpg.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://ygr.jinqigfzy.top


<!-- 参考信息 -->