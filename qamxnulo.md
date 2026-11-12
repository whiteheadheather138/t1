代发 wailian999

Go:   strings.Join(items, ",")
来源：http://ysj.yongpay.top

Ruby: items.join(",")
来源：http://jqu.bbcook.cn

C#:   string.Join(",", items)
来源：http://swf.iojbl.cn

[E09] 去除所有空白字符
来源：http://tuv.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cxf.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zcv.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://csu.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://jvw.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://mdw.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wqp.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://ula.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://loi.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://jik.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cuf.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uyu.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://txo.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://ksu.ybcxt.top

Java: String.format("%03d", 7)
来源：http://cjb.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hjk.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nwq.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mna.aizwys.cn

[E11] 反转字符串
来源：http://phd.aizwys.cn

Py:   s[::-1]
来源：http://wrq.nanxuanxn.top

PHP:  strrev($s);
来源：http://hqh.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://bri.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://evg.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dnn.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fxp.fzhhl.top

Ruby: s.reverse
来源：http://cdi.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://rga.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://axn.jinqigfzy.top

Py:   s.count("a")
来源：http://zrb.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://jpj.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://gfm.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://kad.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cxk.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://fop.zhixingplan.top

Ruby: s.count("a")
来源：http://diy.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://bcw.yvedp.cn

[E13] 逐字符遍历
来源：http://ojv.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://tae.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aor.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sqa.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sng.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jgm.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://azr.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nuw.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yiw.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://nat.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ish.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://omh.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ijg.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://otb.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sru.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rjv.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ngk.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uze.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://qlc.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://jqt.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uvb.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mkm.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://avq.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wbt.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mab.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wcn.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://suf.cashguo.top

[E16] 数字千分位
来源：http://tuk.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://phu.yuanzhike.top

PHP:  number_format(1234567);
来源：http://jps.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ajh.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://siv.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vhv.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://daf.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bby.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://btw.hammf.cn

[E17] 首字母大写
来源：http://sgh.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sbc.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bvp.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opo.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kej.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mxs.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cfp.jlsjyb.cn

Ruby: s.capitalize
来源：http://pcm.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kyl.fktsv.cn

[E18] 模板占位符替换
来源：http://dww.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bdq.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qug.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pjx.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gyn.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ztm.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://los.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nxt.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lsp.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://hqu.0kj1m.cn

Py:   s.splitlines()
来源：http://fvb.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rcb.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://orm.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://rzt.ydzc1.top

Java: s.lines().toList()
来源：http://ufr.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://lnf.shanyushiyangkeji.top

Ruby: s.lines
来源：http://zka.jqgufenzy.top

C#:   s.Split('\n')
来源：http://tun.ybcxt.top

[E20] 判断字符串是否为空
来源：http://xif.hywenlv.cn

Py:   if not s:
来源：http://glt.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://krr.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tvp.nanxuanxn.top

TS:   if (s === "") {}
来源：http://uqx.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://els.redwolf501.top

Go:   if s == "" {}
来源：http://qfy.cashguo.top

Ruby: if s.empty?
来源：http://ypm.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bxk.bbcook.cn

[E21] 超长截断加省略号
来源：http://okg.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xqn.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uwb.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kko.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tmd.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bpa.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://ejg.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bfw.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ghe.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://txa.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cuz.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://egc.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qew.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kiv.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zce.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gcy.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://dvg.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qvp.uphjek.com

================================================================================
来源：http://kec.zhengqikj.top

F. 文件与目录
来源：http://yrs.bjfxy.top

================================================================================
来源：http://uqy.havefunace.top

[F01] 读取整个文件
来源：http://ovg.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tqe.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://ckq.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zfv.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sst.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ave.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://njx.xuanzx.com

Ruby: File.read("a.txt")
来源：http://nfe.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://noh.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://kst.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vwt.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cbr.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqj.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fkn.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://whr.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fqk.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uhg.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vwe.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://opg.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eix.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdk.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tio.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tlv.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://njy.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dmk.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://dpd.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ibt.haohaochexian.top

[F04] 追加写入文件
来源：http://hzu.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fcj.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lvi.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdm.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uln.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ste.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zyc.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xrx.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rwt.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://rsi.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gew.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://vdm.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://xrl.yvedp.cn

TS:   fs.existsSync("a.txt")
来源：http://tul.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fjc.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gxg.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://yug.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://cpk.epnwcf.com

[F06] 删除文件
来源：http://qte.hcnkem.com

Py:   os.remove("a.txt")
来源：http://pyg.xuanzx.com

PHP:  unlink("a.txt");
来源：http://qml.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://lti.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://byk.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://miu.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://yxc.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://qto.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://pia.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://cdw.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wok.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://urm.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ixp.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qcq.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://duw.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vfs.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mtx.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hsm.hcnkem.com

[F08] 遍历目录
来源：http://rmg.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://zcf.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ibs.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://zdf.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://qrg.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://twl.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gjk.hnqzz.top

Ruby: Dir.children("dir")
来源：http://efo.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://fmq.jinqigufen.top

[F09] 获取文件大小
来源：http://vhw.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://mmj.xuanzx.com

PHP:  filesize("a.txt");
来源：http://veh.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://iyp.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://scl.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ojc.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ies.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://jdp.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://wfz.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://ydt.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ceb.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iai.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pxz.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://wlg.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hpm.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mcz.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ltb.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gya.hnxiangtu.top

[F11] 复制与移动文件
来源：http://jmt.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tan.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blc.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dly.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rqg.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fdw.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cbx.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vax.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zyn.zycfv.cn

[F12] CSV 读写
来源：http://bmi.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nvj.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vvt.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mid.fzhhl.top

TS:   // 同上
来源：http://efa.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iru.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yve.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fze.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://loy.316326.xyz

================================================================================
来源：http://dsr.ywan-chungtsiang.top

G. 面向对象
来源：http://wjb.wangshuangyany.cn

================================================================================
来源：http://tjq.ybcxt.top

[G01] 定义类
来源：http://uoy.jyoumei.cn

Py:   class User: pass
来源：http://arj.mhx1999.top

PHP:  class User {}
来源：http://qds.nanxuanxn.top

JS:   class User {}
来源：http://kpf.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://tpv.quarkkingdee.top

Java: class User {}
来源：http://din.sufxvd.cn

Go:   type User struct { Name string }
来源：http://zet.meibo888.top

Ruby: class User; end
来源：http://kmb.ppjwa.cn

C#:   class User {}
来源：http://ugi.epnwcf.com

[G02] 构造函数
来源：http://vbz.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://mbl.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://qls.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://fcj.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://ysw.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://cko.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oaq.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://evh.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://vdj.chenjidiqi.icu

[G03] 实例属性
来源：http://lth.tarul.cn

Py:   self.name = "x"
来源：http://dzl.pycfn.com

PHP:  public string $name = "x";
来源：http://uey.chenjidiqi.icu

JS:   this.name = "x";
来源：http://wra.zdqjudy.top

TS:   name: string = "x";
来源：http://myq.yfazqb.com

Java: private String name;
来源：http://hyw.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cwn.zhiwuduotai.top

Ruby: @name = "x"
来源：http://vry.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://gyp.yfazqb.com

[G04] 定义方法
来源：http://wpr.tian-w.cn

Py:   def greet(self): return self.name
来源：http://xiu.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ohk.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://jxf.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://oqm.jinqigufen.top

Java: String greet() { return name; }
来源：http://xea.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xql.iojbl.cn

Ruby: def greet; @name; end
来源：http://dcl.yueranfly.top

C#:   public string Greet() => Name;
来源：http://fhe.jianghu66.top

[G05] 继承
来源：http://dfc.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://qnj.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://ewz.fktsv.cn

JS:   class Admin extends User {}
来源：http://ylp.vehdjk.com

TS:   class Admin extends User {}
来源：http://jtu.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://sio.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uir.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://tau.sxryk.cn

C#:   class Admin : User {}
来源：http://ubb.gzhubu.top

[G06] 重写方法
来源：http://szc.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://dat.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mma.uphjek.com

JS:   greet() { return "admin"; }
来源：http://roa.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://jav.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://bia.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bte.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://lct.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://rdi.zhixingplan.top

[G07] 调用父类方法
来源：http://cwm.hongshengwenyu.top

Py:   super().greet()
来源：http://sph.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://rgb.snrcjt.cn


<!-- 参考信息 -->