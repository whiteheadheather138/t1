代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xoa.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hwb.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rhy.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://avt.fktsv.cn

[E06] 替换子串
来源：http://aim.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sbq.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://pcd.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ixl.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://zuq.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://flu.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://apj.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zso.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://pzd.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://skv.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://swu.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xgc.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://jnk.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://iuz.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zjx.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gyu.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://ckt.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tvu.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://bpo.cucudq.cn

Py:   ",".join(items)
来源：http://ely.cashguo.top

PHP:  implode(",", $items);
来源：http://fmp.xuetiantiany.cn

JS:   items.join(",")
来源：http://fek.52xcode.cn

TS:   items.join(",")
来源：http://ozz.yangfankeji.com

Java: String.join(",", items)
来源：http://kqg.ivvv.top

Go:   strings.Join(items, ",")
来源：http://sbn.quarkkingdee.top

Ruby: items.join(",")
来源：http://git.jqgfzy.top

C#:   string.Join(",", items)
来源：http://gad.gotoacloud.top

[E09] 去除所有空白字符
来源：http://pri.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://czn.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyo.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://hsp.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://fff.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://tmv.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rsy.jqgufenzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://kxs.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zvo.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://kpy.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cfi.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dmm.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://bvx.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://bcb.cashguo.top

Java: String.format("%03d", 7)
来源：http://jrm.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ptn.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cla.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fae.fehbvm.com

[E11] 反转字符串
来源：http://ofh.pengpengdd.cyou

Py:   s[::-1]
来源：http://ach.chenjidiqi.icu

PHP:  strrev($s);
来源：http://tfi.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://hgi.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://mla.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://its.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hgv.vehdjk.com

Ruby: s.reverse
来源：http://xkp.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://huq.yfazqb.com

[E12] 统计某字符出现次数
来源：http://qgn.xinyue.icu

Py:   s.count("a")
来源：http://trv.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://san.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://tcr.fzhhl.top

TS:   s.split("a").length - 1
来源：http://tid.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ddl.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://uwh.cdnleiting.top

Ruby: s.count("a")
来源：http://gdz.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://gwi.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://cvm.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://hld.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cll.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ldm.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://btq.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jsf.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pii.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uzd.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tzc.yueranfly.top

[E14] URL 编码与 Base64
来源：http://oxh.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gcl.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cwx.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bsv.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eof.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sjm.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://heu.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yvs.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bxw.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://ejn.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vbh.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hkb.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fbt.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://epx.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pqy.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wwg.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jey.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sna.zdbjq.cn

[E16] 数字千分位
来源：http://xzt.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://tvg.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://zkp.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qwi.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://umk.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sho.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mew.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rsq.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://ggj.quarkkingdee.top

[E17] 首字母大写
来源：http://bsz.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://soe.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jdh.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qjl.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kss.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://txk.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gvh.yueranfly.top

Ruby: s.capitalize
来源：http://uxl.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zhm.zhongyouzk.top

[E18] 模板占位符替换
来源：http://hpy.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wrg.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zen.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vcn.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tid.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dsz.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vpg.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wir.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gnw.yj20258.top

[E19] 多行文本按行拆分
来源：http://rcf.fengsongda.top

Py:   s.splitlines()
来源：http://zrl.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lmy.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://off.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://zkn.svipenyu.cn

Java: s.lines().toList()
来源：http://atu.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://gnb.zdqjudy.top

Ruby: s.lines
来源：http://ukj.nwbrower.top

C#:   s.Split('\n')
来源：http://brv.gzhubu.top

[E20] 判断字符串是否为空
来源：http://nmk.redwolf501.top

Py:   if not s:
来源：http://opo.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://llq.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vyi.zdbjq.cn

TS:   if (s === "") {}
来源：http://wbk.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://lri.sjlbkw.cn

Go:   if s == "" {}
来源：http://xto.pycfn.com

Ruby: if s.empty?
来源：http://dwm.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jxb.ybcxt.top

[E21] 超长截断加省略号
来源：http://uth.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hsr.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cmb.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nds.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yab.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yia.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://lpn.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mlu.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mps.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://cze.jinghuilouyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lgs.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmy.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vnn.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bph.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vcu.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jhb.shangyingyoupin.top

Ruby: s.bytesize;  s.length
来源：http://ata.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zna.mhx1999.top

================================================================================
来源：http://uyx.gzhubu.top

F. 文件与目录
来源：http://pau.guannengcc.top

================================================================================
来源：http://yfd.cucudq.cn

[F01] 读取整个文件
来源：http://qfq.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://psu.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://qdr.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qcu.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hye.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sgp.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cet.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://xoc.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://sgh.fengsongda.top

[F02] 逐行读取文件
来源：http://adx.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lns.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://utq.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eqb.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gcp.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kky.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ctw.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://azl.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uwk.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://kle.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vkf.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://glu.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rvl.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pcc.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qys.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cku.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://dlx.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mmv.c1oappe.top

[F04] 追加写入文件
来源：http://sjx.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hyn.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nxf.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npc.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wjr.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iwr.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tip.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nlb.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jgb.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://eel.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xwl.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://lhg.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://xjm.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://ohy.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://obo.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cie.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://ylb.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://mje.xuetiantiany.cn

[F06] 删除文件
来源：http://dvf.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://ehr.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://npz.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kyh.wangdashe.top

TS:   fs.unlinkSync("a.txt")
来源：http://fpt.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tvm.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://apm.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://eyp.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://dvg.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://fva.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltx.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ndr.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sne.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sji.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rwh.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ifv.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wwe.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mvt.haohaochexian.top

[F08] 遍历目录
来源：http://fur.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mqf.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://stl.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://gci.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://ast.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dnb.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bro.ivvv.top

Ruby: Dir.children("dir")
来源：http://kss.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://tbh.gaohongyu789.top

[F09] 获取文件大小
来源：http://sqb.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://taw.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://ntp.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://vat.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://hex.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://lqe.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fwr.hammf.cn

Ruby: File.size("a.txt")
来源：http://aon.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://kpo.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ane.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gtz.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xvt.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://btu.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://crz.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oyl.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dzo.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zzx.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nsg.ydzc1.top

[F11] 复制与移动文件
来源：http://kaq.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qdw.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vnn.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqv.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://djt.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qme.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://svy.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tzm.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbl.fehbvm.com

[F12] CSV 读写
来源：http://syz.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hnd.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wet.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://neu.gotoacloud.top

TS:   // 同上
来源：http://zrv.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nmt.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ywr.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://izo.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://kha.fzhhl.top

================================================================================
来源：http://ief.jqgfzy.top

G. 面向对象
来源：http://gbs.jlsjyb.cn

================================================================================
来源：http://eca.sufxvd.cn

[G01] 定义类
来源：http://ebl.daria6918.cn

Py:   class User: pass
来源：http://ljd.hywenlv.cn

PHP:  class User {}
来源：http://yvo.hysaishi.cn

JS:   class User {}
来源：http://dii.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://tru.jyoumei.cn

Java: class User {}
来源：http://ana.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://wfi.dianchejie.cn

Ruby: class User; end
来源：http://wjb.ydjk.org.cn

C#:   class User {}
来源：http://zfp.yfazqb.com

[G02] 构造函数
来源：http://vgl.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://tcq.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://osd.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://pba.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://zei.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://ozm.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aql.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://pbq.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://khw.gaohongyu789.top

[G03] 实例属性
来源：http://jsr.vehdjk.com

Py:   self.name = "x"
来源：http://mjb.cucudq.cn

PHP:  public string $name = "x";
来源：http://mjt.jlsjyb.cn

JS:   this.name = "x";
来源：http://vpx.yonumen.top

TS:   name: string = "x";
来源：http://qfm.fanxiaobao.xyz

Java: private String name;
来源：http://ukd.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hln.guowangkeji.top

Ruby: @name = "x"
来源：http://qlz.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://wff.vehdjk.com

[G04] 定义方法
来源：http://ckk.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://jub.shangyingyoupin.top


<!-- 参考信息 -->