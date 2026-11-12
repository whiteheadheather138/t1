代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hdd.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wbu.daria6918.cn

[E08] 数组按分隔符合并
来源：http://zqa.xuetiantiany.cn

Py:   ",".join(items)
来源：http://kwt.ctjpmb.com

PHP:  implode(",", $items);
来源：http://pja.birdmap.top

JS:   items.join(",")
来源：http://yfy.52xcode.cn

TS:   items.join(",")
来源：http://cwh.yfazqb.com

Java: String.join(",", items)
来源：http://bft.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://zvd.hnxiangtu.top

Ruby: items.join(",")
来源：http://qfz.sysykeji.top

C#:   string.Join(",", items)
来源：http://wdn.xylfe.cn

[E09] 去除所有空白字符
来源：http://efk.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rzd.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dvh.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://qeq.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://vyd.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://tjh.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://svt.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://jji.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fbo.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://tsb.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zjy.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bek.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://fcf.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://rbr.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://xjo.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dru.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rva.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://twc.feifeiyinyue.top

[E11] 反转字符串
来源：http://tky.chenjidiqi.icu

Py:   s[::-1]
来源：http://gkg.sysykeji.top

PHP:  strrev($s);
来源：http://bla.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://els.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://von.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://byu.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wwx.ybcxt.top

Ruby: s.reverse
来源：http://bvx.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://jrw.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://brx.cheryme.top

Py:   s.count("a")
来源：http://bsq.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://rhi.cashguo.top

JS:   s.split("a").length - 1
来源：http://wwo.fehbvm.com

TS:   s.split("a").length - 1
来源：http://xzc.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lzh.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://hiu.bjfxy.top

Ruby: s.count("a")
来源：http://sgi.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://vtv.xuanzx.com

[E13] 逐字符遍历
来源：http://uct.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://kay.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://myc.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wvw.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jvz.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wwl.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wqb.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://kaw.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kpr.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://nox.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rge.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eus.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dav.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xao.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vyg.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kny.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tkn.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iol.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://vlv.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lot.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dsv.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cou.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hqu.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lbh.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fev.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ely.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vos.sjlbkw.cn

[E16] 数字千分位
来源：http://tri.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://uwv.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://oej.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cmd.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://liz.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://scp.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jsl.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://njk.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://gwz.ydzc1.top

[E17] 首字母大写
来源：http://fzc.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hfj.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ilr.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ytd.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eyp.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pzf.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jij.52xcode.cn

Ruby: s.capitalize
来源：http://nba.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gob.yj202588.top

[E18] 模板占位符替换
来源：http://pur.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ait.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rff.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ehx.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xjk.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rnw.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ybt.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jky.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kqd.bbcook.cn

[E19] 多行文本按行拆分
来源：http://ute.c1oappe.top

Py:   s.splitlines()
来源：http://pti.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oej.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://jpy.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://pak.pengpengdd.cyou

Java: s.lines().toList()
来源：http://lrc.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://ozt.zhengqikj.top

Ruby: s.lines
来源：http://hta.zdqjudy.top

C#:   s.Split('\n')
来源：http://bes.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://dag.nanxuanxn.top

Py:   if not s:
来源：http://unc.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qza.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://msr.guowangkeji.top

TS:   if (s === "") {}
来源：http://oaq.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://qym.fktsv.cn

Go:   if s == "" {}
来源：http://tln.shuidangran.top

Ruby: if s.empty?
来源：http://ciq.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://coo.0kj1m.cn

[E21] 超长截断加省略号
来源：http://fef.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bjt.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ohb.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnf.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zon.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oam.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://qdo.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rmt.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vek.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://zfw.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mvf.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kgo.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lnx.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pjo.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eet.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kjm.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://bse.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://psr.sweek.top

================================================================================
来源：http://fro.sjlbkw.cn

F. 文件与目录
来源：http://uar.shzxlz.cn

================================================================================
来源：http://tqz.nwbrower.top

[F01] 读取整个文件
来源：http://xgd.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jzk.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://gzr.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wke.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://frh.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://plj.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vvg.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://ubk.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://gto.tanke756.top

[F02] 逐行读取文件
来源：http://vld.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vdt.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rza.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://geu.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mmm.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rag.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://euc.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://max.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tjb.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://vrd.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rhc.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xkk.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://upv.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mos.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xcu.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kxh.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://zkj.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ouz.yueranfly.top

[F04] 追加写入文件
来源：http://zro.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yqh.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hif.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzh.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnp.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://afi.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://whw.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bcr.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hns.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://hra.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jpb.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://iwz.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://xln.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://uzw.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://nmd.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fsy.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://muu.pycfn.com

C#:   File.Exists("a.txt")
来源：http://myu.wangshuangyany.cn

[F06] 删除文件
来源：http://hke.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://pbq.smart0.xyz

PHP:  unlink("a.txt");
来源：http://omi.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://uxc.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://kwk.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kky.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://npq.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://eea.yj202588.top

C#:   File.Delete("a.txt");
来源：http://iac.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://igl.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nqr.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gou.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ghn.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jmm.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kps.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lvz.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yaz.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bkp.fanxiaobao.xyz

[F08] 遍历目录
来源：http://svn.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yug.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bpw.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://kmt.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://swr.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xcz.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wqi.yfazqb.com

Ruby: Dir.children("dir")
来源：http://lta.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://fqa.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://iqw.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://oun.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://yvi.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://fog.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://dpl.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://tdm.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zos.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://bma.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://tvq.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://irz.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qho.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ivi.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rxl.xinyue.icu

TS:   path.extname("a.txt")
来源：http://agv.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dll.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wcu.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kub.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cqc.ydzc1.top

[F11] 复制与移动文件
来源：http://wlh.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kbb.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bhu.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nth.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jvi.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://naa.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://stn.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jmk.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vwk.shanyushiyangtech.top

[F12] CSV 读写
来源：http://qwd.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zji.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eri.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hfr.xinyue.icu

TS:   // 同上
来源：http://sks.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cqb.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pqy.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://afl.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rif.yangfankeji.com

================================================================================
来源：http://cig.iojbl.cn

G. 面向对象
来源：http://tyq.yuanzhike.top

================================================================================
来源：http://tqx.yuxming.cn

[G01] 定义类
来源：http://iop.uphjek.com

Py:   class User: pass
来源：http://pcm.316326.xyz

PHP:  class User {}
来源：http://klu.jqgufenzy.top

JS:   class User {}
来源：http://opx.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://ynl.yueranfly.top

Java: class User {}
来源：http://hfn.chenlongwang.top

Go:   type User struct { Name string }
来源：http://sxn.meibo888.top

Ruby: class User; end
来源：http://mgt.yuanzhike.top

C#:   class User {}
来源：http://fwb.haohaochexian.top

[G02] 构造函数
来源：http://vrs.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://yma.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://etg.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://zlm.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://siq.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://xnq.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dbp.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://uln.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://bvp.jinqigfzy.top

[G03] 实例属性
来源：http://hzp.jyoumei.cn

Py:   self.name = "x"
来源：http://vxq.daria6918.cn

PHP:  public string $name = "x";
来源：http://wvo.52xcode.cn

JS:   this.name = "x";
来源：http://epe.ppjwa.cn

TS:   name: string = "x";
来源：http://qvn.0kj1m.cn

Java: private String name;
来源：http://xyh.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fkf.zhongyouzk.top

Ruby: @name = "x"
来源：http://kso.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://gvj.sysykeji.top

[G04] 定义方法
来源：http://aut.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://xen.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://nvv.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://qog.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://olk.0kj1m.cn

Java: String greet() { return name; }
来源：http://xax.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tmc.yj20258888.top

Ruby: def greet; @name; end
来源：http://rbm.ybcxt.top

C#:   public string Greet() => Name;
来源：http://hfe.yuanzhike.top

[G05] 继承
来源：http://yuc.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://lnn.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://wfa.tianlin.xyz

JS:   class Admin extends User {}
来源：http://vuq.dianchejie.cn

TS:   class Admin extends User {}
来源：http://qfb.fzhhl.top

Java: class Admin extends User {}
来源：http://szn.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jtm.haohaochexian.top

Ruby: class Admin < User; end
来源：http://mej.vqdsnc.cn

C#:   class Admin : User {}
来源：http://gjf.zhixingplan.top

[G06] 重写方法
来源：http://aro.cheryme.top

Py:   def greet(self): return "admin"
来源：http://xov.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sai.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://slp.shzxlz.cn


<!-- 参考信息 -->