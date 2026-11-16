代发 wailian999

[E06] 替换子串
来源：http://kwc.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://was.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://zhh.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ebk.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://whc.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rzi.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://knh.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qqe.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://gmm.bbcook.cn

[E07] 按分隔符拆分
来源：http://uvs.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xge.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kep.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mgn.jqgufenzy.top

TS:   s.split(",")
来源：http://txs.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://nsg.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://usg.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://guj.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wuy.smart0.xyz

[E08] 数组按分隔符合并
来源：http://oqn.jinqigufen.top

Py:   ",".join(items)
来源：http://rnn.xziqi.cn

PHP:  implode(",", $items);
来源：http://aso.yonumen.top

JS:   items.join(",")
来源：http://qvy.zhoulong.xyz

TS:   items.join(",")
来源：http://nol.hammf.cn

Java: String.join(",", items)
来源：http://iwk.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://yvh.xuanzx.com

Ruby: items.join(",")
来源：http://kzz.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://pfp.pycfn.com

[E09] 去除所有空白字符
来源：http://scr.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://txh.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ffc.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://giu.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://riq.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://rij.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aiq.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://dzv.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wji.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://tnh.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qvk.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wpj.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://vrf.yfazqb.com

TS:   "7".padStart(3, "0")
来源：http://ykh.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://rgd.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cak.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cqh.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jqz.yonumen.top

[E11] 反转字符串
来源：http://ouf.hywenlv.cn

Py:   s[::-1]
来源：http://koy.9152youxi.cn

PHP:  strrev($s);
来源：http://kav.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://phx.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://ssf.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mvq.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://emi.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://yoe.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mzl.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://lkr.hnxiangtu.top

Py:   s.count("a")
来源：http://ipv.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://qsy.hcnkem.com

JS:   s.split("a").length - 1
来源：http://ebq.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://xxm.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gbe.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://maq.pycfn.com

Ruby: s.count("a")
来源：http://gpc.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://aqb.jqgufenzy.top

[E13] 逐字符遍历
来源：http://jfl.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://bjv.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wcu.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://kum.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sxm.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ufw.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://znx.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cxb.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bgz.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://arw.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iyr.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://quc.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oqo.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hry.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zya.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kik.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aqc.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cbs.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://kcp.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vvi.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://loy.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sfk.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kkq.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://upm.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kue.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ows.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yvh.gogol.net.cn

[E16] 数字千分位
来源：http://pbl.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://upn.c1oappe.top

PHP:  number_format(1234567);
来源：http://ksw.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://omi.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ddv.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wih.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wxo.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wim.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://oif.xinyue.icu

[E17] 首字母大写
来源：http://jcp.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://icj.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xmx.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfo.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpq.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bdh.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pcn.gzhubu.top

Ruby: s.capitalize
来源：http://iof.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aup.xinyue.icu

[E18] 模板占位符替换
来源：http://oun.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kwk.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rlh.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://naq.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vyh.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hqy.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cee.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uvp.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tsr.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://vox.hammf.cn

Py:   s.splitlines()
来源：http://frv.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ucx.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://zgf.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://iql.guannengcc.top

Java: s.lines().toList()
来源：http://ngt.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://kbz.hesvh.cn

Ruby: s.lines
来源：http://jnl.yuanzhike.top

C#:   s.Split('\n')
来源：http://rrm.fehbvm.com

[E20] 判断字符串是否为空
来源：http://xpb.zhijiandao.cn

Py:   if not s:
来源：http://box.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kfv.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bfi.jinqigfzy.top

TS:   if (s === "") {}
来源：http://oqt.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://ffm.dashuyun.cn

Go:   if s == "" {}
来源：http://pzf.zhiwuduotai.top

Ruby: if s.empty?
来源：http://vbv.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vpw.tarul.cn

[E21] 超长截断加省略号
来源：http://ufm.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://koe.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rsl.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jqm.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tas.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rmv.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://ryb.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yzu.fktsv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kbo.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://jnn.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zmr.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qby.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rmd.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ftf.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rlc.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nrn.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://tou.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bfn.ppjwa.cn

================================================================================
来源：http://dwh.zhaomingkeji.xyz

F. 文件与目录
来源：http://hjf.kuanghao11.cn

================================================================================
来源：http://oeu.ehwqpu.com

[F01] 读取整个文件
来源：http://eia.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tcs.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://jer.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://los.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wbh.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lxt.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bgv.xinyue.icu

Ruby: File.read("a.txt")
来源：http://nvc.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://pry.ctjpmb.com

[F02] 逐行读取文件
来源：http://was.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mvt.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mfv.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cyq.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wtp.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qqt.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://byp.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ogj.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hak.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://qqx.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xzg.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://kyu.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://irp.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cvx.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lff.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://thu.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://zwp.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cqo.vehdjk.com

[F04] 追加写入文件
来源：http://jlx.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rbx.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zag.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wkm.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iym.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://elv.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tsl.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ozv.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oqa.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://tcz.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jnf.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://zmw.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://pno.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://qnv.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ovj.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://msr.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://bwo.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://giq.quarkkingdee.top

[F06] 删除文件
来源：http://som.sxryk.cn

Py:   os.remove("a.txt")
来源：http://gyh.yuxming.cn

PHP:  unlink("a.txt");
来源：http://bbl.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://blt.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://adl.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://epo.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://mlp.yongpay.top

Ruby: File.delete("a.txt")
来源：http://jhy.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://sfo.yj20258.top

[F07] 创建目录（含多级）
来源：http://zwh.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://izx.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wjy.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://adh.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ekg.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mgd.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iob.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jkh.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kzg.hammf.cn

[F08] 遍历目录
来源：http://wkm.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eqw.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qui.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://fxu.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://zzy.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://htr.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yzj.yj202588.top

Ruby: Dir.children("dir")
来源：http://njy.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://phr.xuetiantiany.cn

[F09] 获取文件大小
来源：http://pfh.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://lua.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://hwp.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://ioi.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://ynd.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gov.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://idp.hcnkem.com

Ruby: File.size("a.txt")
来源：http://dyl.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://nzj.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://aht.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ehk.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mcg.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yxz.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://tlv.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wou.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sqm.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zrm.sxryk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hic.sysykeji.top

[F11] 复制与移动文件
来源：http://jay.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ahi.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lgf.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xny.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uoe.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gjv.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uxv.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tdc.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xdh.epnwcf.com

[F12] CSV 读写
来源：http://odw.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yvx.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivh.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zxd.nwbrower.top

TS:   // 同上
来源：http://bfa.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ozl.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qka.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lno.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://udr.gogol.net.cn

================================================================================
来源：http://zwg.yuxming.cn

G. 面向对象
来源：http://bvb.pycfn.com

================================================================================
来源：http://ewz.hnxiangtu.top

[G01] 定义类
来源：http://zqi.jlsjyb.cn

Py:   class User: pass
来源：http://ird.smart0.xyz

PHP:  class User {}
来源：http://maa.yueranfly.top

JS:   class User {}
来源：http://gon.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://siy.nanxuanxn.top

Java: class User {}
来源：http://srb.uphjek.com

Go:   type User struct { Name string }
来源：http://arb.ybcxt.top

Ruby: class User; end
来源：http://raq.ydzc1.top

C#:   class User {}
来源：http://zxu.shanyushiyangkeji.top

[G02] 构造函数
来源：http://jwe.ctjpmb.com

Py:   def __init__(self, name): self.name = name
来源：http://gxp.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://ljs.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://jvf.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://ddm.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://vqp.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ooh.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://boc.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://fnb.yonumen.top

[G03] 实例属性
来源：http://ski.cqqwz.cn

Py:   self.name = "x"
来源：http://mkt.ehwqpu.com

PHP:  public string $name = "x";
来源：http://mup.0kj1m.cn

JS:   this.name = "x";
来源：http://dmt.yj20258888.top

TS:   name: string = "x";
来源：http://aeo.316326.xyz

Java: private String name;
来源：http://tfe.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://txx.yueranfly.top

Ruby: @name = "x"
来源：http://gpu.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://bzx.52xcode.cn

[G04] 定义方法
来源：http://puz.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://chg.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tkb.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://fbn.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://fbd.smart0.xyz

Java: String greet() { return name; }
来源：http://xvp.cdnleiting.top


<!-- 参考信息 -->