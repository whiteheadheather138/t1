代发 wailian999

Ruby: s.split(",");  s.split
来源：http://qld.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://szo.wangdashe.top

[E08] 数组按分隔符合并
来源：http://ljd.xuanzx.com

Py:   ",".join(items)
来源：http://tdt.yj20258888.top

PHP:  implode(",", $items);
来源：http://ojs.epnwcf.com

JS:   items.join(",")
来源：http://lic.mhx1999.top

TS:   items.join(",")
来源：http://egb.daria6918.cn

Java: String.join(",", items)
来源：http://lab.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://ngh.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://wwd.havefunace.top

C#:   string.Join(",", items)
来源：http://swf.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://zig.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyb.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vnj.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://inc.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://vno.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://ngd.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rnu.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ckp.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ksk.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://njz.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hea.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dmj.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://owo.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://fov.mhx1999.top

Java: String.format("%03d", 7)
来源：http://xfa.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://elh.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ofm.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://msj.feifeiyinyue.top

[E11] 反转字符串
来源：http://xqk.zdbjq.cn

Py:   s[::-1]
来源：http://dxy.sxryk.cn

PHP:  strrev($s);
来源：http://lst.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://gvr.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://bdf.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://yoo.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rsk.dianchejie.cn

Ruby: s.reverse
来源：http://tvl.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ixv.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://tgp.daria6918.cn

Py:   s.count("a")
来源：http://egq.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://kxh.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://qaw.mhx1999.top

TS:   s.split("a").length - 1
来源：http://auo.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cwv.uphjek.com

Go:   strings.Count(s, "a")
来源：http://dii.aibaodan.cn

Ruby: s.count("a")
来源：http://aqh.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://flx.bbcook.cn

[E13] 逐字符遍历
来源：http://iuw.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://rcl.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kno.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxo.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://avd.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cta.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tgx.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bbh.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fzi.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://msx.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ukb.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mkg.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svi.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://txm.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ltp.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nhx.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gjf.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kbs.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://lro.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://pmi.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rvo.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yuq.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rqm.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rpz.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uiw.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cet.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mnc.c1oappe.top

[E16] 数字千分位
来源：http://ita.pycfn.com

Py:   f"{1234567:,}"
来源：http://dja.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://vdl.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jqs.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://sru.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wnu.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xox.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mce.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://uvs.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://lfl.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sin.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cap.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://byy.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://trd.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://syd.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iio.kuanghao11.cn

Ruby: s.capitalize
来源：http://cvn.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxa.sweek.top

[E18] 模板占位符替换
来源：http://csx.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zyk.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://man.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uvl.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vgq.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vfn.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://leh.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iac.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zha.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://iwh.ybcxt.top

Py:   s.splitlines()
来源：http://axc.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mop.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://hns.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://cdp.0kj1m.cn

Java: s.lines().toList()
来源：http://xja.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://zth.yuanzhike.top

Ruby: s.lines
来源：http://vok.hfpthk.cn

C#:   s.Split('\n')
来源：http://giw.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://stl.hesvh.cn

Py:   if not s:
来源：http://wzh.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dgp.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wua.316326.xyz

TS:   if (s === "") {}
来源：http://jnn.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://bpd.sweek.top

Go:   if s == "" {}
来源：http://tza.hesvh.cn

Ruby: if s.empty?
来源：http://okt.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dwb.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://tgb.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tvp.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qzl.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ntb.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://atn.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dmc.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://uoz.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cww.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iaq.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://tfi.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bpq.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytz.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://inn.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dnt.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bhb.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nml.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://gdt.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sfq.aizwys.cn

================================================================================
来源：http://bsc.tianlin.xyz

F. 文件与目录
来源：http://inc.guowangkeji.top

================================================================================
来源：http://srp.yuanzhike.top

[F01] 读取整个文件
来源：http://hfa.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uxe.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://msa.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ofd.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ekc.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nbz.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ehp.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://nwp.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://svv.yj20258888.top

[F02] 逐行读取文件
来源：http://aqv.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cwq.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pcw.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qeb.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://trc.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgl.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mls.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jam.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zir.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://tmz.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cyi.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://phj.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://opo.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbb.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rnn.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://waz.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://ypm.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dvj.yuanzhike.top

[F04] 追加写入文件
来源：http://ghg.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hst.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cfi.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lgx.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhw.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gtq.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iqw.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://goa.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mnw.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://cvd.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nqy.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://rvf.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://iob.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://zep.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cka.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lyx.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://nfs.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://ciy.gotoacloud.top

[F06] 删除文件
来源：http://syw.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://dvw.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://jpr.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://oob.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://awd.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kgt.cashguo.top

Go:   os.Remove("a.txt")
来源：http://leb.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://sif.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://jeo.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://mqf.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://npj.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dyr.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tjn.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpq.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oba.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kru.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ddx.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ldk.wangdashe.top

[F08] 遍历目录
来源：http://gss.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hun.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fro.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://wkj.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://qoh.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fub.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gsd.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://ook.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://xbq.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://aka.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://vja.smart0.xyz

PHP:  filesize("a.txt");
来源：http://zpm.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://gxo.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://dqa.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://sgw.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://emk.52xcode.cn

Ruby: File.size("a.txt")
来源：http://rqo.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://jnq.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqh.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xky.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fqa.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uqq.c1oappe.top

TS:   path.extname("a.txt")
来源：http://lbn.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://alx.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://njk.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://teq.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bcd.svipenyu.cn

[F11] 复制与移动文件
来源：http://yct.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://otz.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baq.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fdn.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://txi.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cru.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://byk.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://axi.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rhx.uphjek.com

[F12] CSV 读写
来源：http://tvb.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ibh.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nbs.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ykl.zhengqikj.top

TS:   // 同上
来源：http://hhd.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ijs.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://snt.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jth.dashuyun.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gcg.jinghuilouyu.cn

================================================================================
来源：http://nuv.yj202588.top

G. 面向对象
来源：http://gou.gaohongyu789.top

================================================================================
来源：http://gmw.yanxiufei.cn

[G01] 定义类
来源：http://dqq.zdqjudy.top

Py:   class User: pass
来源：http://cla.snrcjt.cn

PHP:  class User {}
来源：http://les.yuanzhike.top

JS:   class User {}
来源：http://bcg.cheryme.top

TS:   class User { name: string = ""; }
来源：http://zna.zhaomingkeji.xyz

Java: class User {}
来源：http://hmn.yvedp.cn

Go:   type User struct { Name string }
来源：http://dgj.kuanghao11.cn

Ruby: class User; end
来源：http://ryt.yj20258.top

C#:   class User {}
来源：http://nka.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://zyh.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://ehl.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://pqd.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://rny.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://qxz.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://rdu.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jak.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://fne.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://dev.hnqzz.top

[G03] 实例属性
来源：http://mly.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://cnj.daria6918.cn

PHP:  public string $name = "x";
来源：http://oma.wangdashe.top

JS:   this.name = "x";
来源：http://cow.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://aju.aizwys.cn

Java: private String name;
来源：http://pzv.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://igz.chenjidiqi.icu

Ruby: @name = "x"
来源：http://xtc.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://xar.ywan-chungtsiang.top

[G04] 定义方法
来源：http://nfx.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://vmr.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cyd.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://ycd.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://yws.c1oappe.top

Java: String greet() { return name; }
来源：http://wes.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://uto.xylfe.cn

Ruby: def greet; @name; end
来源：http://oti.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://jkq.hesvh.cn

[G05] 继承
来源：http://dge.ybcxt.top

Py:   class Admin(User): pass
来源：http://cau.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://uee.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://haa.yvedp.cn

TS:   class Admin extends User {}
来源：http://mgu.fengsongda.top

Java: class Admin extends User {}
来源：http://vur.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cel.yonumen.top

Ruby: class Admin < User; end
来源：http://egr.shzxlz.cn

C#:   class Admin : User {}
来源：http://gow.zhaomingkeji.xyz

[G06] 重写方法
来源：http://fxl.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://cgl.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pyz.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://ygw.fengsongda.top


<!-- 参考信息 -->