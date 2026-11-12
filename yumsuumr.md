代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mox.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fmj.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nur.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zng.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tzd.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yni.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kia.sxryk.cn

[D26] 数组转字符串
来源：http://pgj.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://mng.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://lwz.zhengqikj.top

JS:   arr.join(", ")
来源：http://exb.cucudq.cn

TS:   arr.join(", ")
来源：http://upu.fktsv.cn

Java: String.join(", ", list)
来源：http://xyq.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://tgd.jianghu66.top

Ruby: arr.join(", ")
来源：http://jyi.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://tgz.guannengcc.top

================================================================================
来源：http://bvm.nanxuanxn.top

E. 字符串处理
来源：http://rpc.vqdsnc.cn

================================================================================
来源：http://sqd.tanke756.top

[E01] 拼接字符串
来源：http://vqr.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zvc.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hhb.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://umg.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iux.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://doe.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://atz.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qoq.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vqu.zhoulong.xyz

[E02] 重复字符串
来源：http://epx.xinyue.icu

Py:   "ab" * 3
来源：http://vqn.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://efv.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://ctr.zycfv.cn

TS:   "ab".repeat(3)
来源：http://vlw.tianlin.xyz

Java: "ab".repeat(3)
来源：http://qvx.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://fpu.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://bhp.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oov.iojbl.cn

[E03] 截取子串
来源：http://ufc.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eji.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kxc.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wuc.birdmap.top

TS:   s.slice(1, 4)
来源：http://snt.gzhubu.top

Java: s.substring(1, 4)
来源：http://opx.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jgd.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://jsj.316326.xyz

C#:   s.Substring(1, 3)
来源：http://dar.wangshuangyany.cn

[E04] 查找子串位置
来源：http://ldo.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://zju.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://kbf.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngo.yuxming.cn

TS:   s.indexOf("x")
来源：http://fff.ppjwa.cn

Java: s.indexOf("x")
来源：http://kvm.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://xvh.redwolf501.top

Ruby: s.index("x")
来源：http://zma.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://sxe.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xvz.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xof.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhv.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbo.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oda.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hsz.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dxr.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gmw.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bzh.jinghuilouyu.cn

[E06] 替换子串
来源：http://pcb.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zxi.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://bsf.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llm.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://sri.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mof.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ofz.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://col.yongpay.top

C#:   s.Replace("a", "b")
来源：http://spu.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://rrs.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ciz.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xea.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qvr.cdnleiting.top

TS:   s.split(",")
来源：http://vav.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nht.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eoc.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://fil.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aax.nwbrower.top

[E08] 数组按分隔符合并
来源：http://eli.xuetiantiany.cn

Py:   ",".join(items)
来源：http://dtn.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://uwh.birdmap.top

JS:   items.join(",")
来源：http://wxq.feifeiyinyue.top

TS:   items.join(",")
来源：http://ggt.nanxuanxn.top

Java: String.join(",", items)
来源：http://lyd.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://ocl.chenlongwang.top

Ruby: items.join(",")
来源：http://rhq.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://amv.hfpthk.cn

[E09] 去除所有空白字符
来源：http://kvl.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lye.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lul.wangshuangyany.cn

JS:   s.replace(/\s+/g, "")
来源：http://asl.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://tcg.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://mve.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iyy.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://oej.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wtb.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://zkc.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ixz.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uiy.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://uil.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://xsy.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://kcd.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://piw.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rrb.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qof.chenzaomai.com

[E11] 反转字符串
来源：http://viz.fktsv.cn

Py:   s[::-1]
来源：http://jzs.yongpay.top

PHP:  strrev($s);
来源：http://qvj.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://ban.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://vfd.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zxn.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://skx.vehdjk.com

Ruby: s.reverse
来源：http://tbl.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://fgi.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://qmw.gotoacloud.top

Py:   s.count("a")
来源：http://hzg.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://dwv.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://ybg.316326.xyz

TS:   s.split("a").length - 1
来源：http://ghn.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gqs.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://suf.xylfe.cn

Ruby: s.count("a")
来源：http://hrk.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://cdn.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://rvw.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://viu.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zdu.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ntu.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://tgr.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dhv.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aww.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bfx.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pie.guannengcc.top

[E14] URL 编码与 Base64
来源：http://qun.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vtg.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qhh.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mpu.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fia.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fej.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tnd.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hju.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wgg.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://det.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://amx.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://drh.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kvc.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kyj.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fpg.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hkv.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wjx.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vyv.9152youxi.cn

[E16] 数字千分位
来源：http://hmw.xinyue.icu

Py:   f"{1234567:,}"
来源：http://ndm.ivvv.top

PHP:  number_format(1234567);
来源：http://sbh.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://svo.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jay.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lpw.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tio.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mmb.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://bag.quarkkingdee.top

[E17] 首字母大写
来源：http://pch.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yaq.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jac.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umz.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdc.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rch.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cyt.hfpthk.cn

Ruby: s.capitalize
来源：http://kqj.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sjj.sysykeji.top

[E18] 模板占位符替换
来源：http://mmu.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://etq.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://owc.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gjj.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hbo.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uzr.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ndo.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yoi.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mzj.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://ngg.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://mcu.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vai.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://vli.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://qin.cucudq.cn

Java: s.lines().toList()
来源：http://xzf.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://nmd.cashguo.top

Ruby: s.lines
来源：http://yck.jlsjyb.cn

C#:   s.Split('\n')
来源：http://ncl.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://aog.ydzc1.top

Py:   if not s:
来源：http://ogh.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eeb.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxo.nwbrower.top

TS:   if (s === "") {}
来源：http://mzb.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://avq.9152youxi.cn

Go:   if s == "" {}
来源：http://suz.yj20258888.top

Ruby: if s.empty?
来源：http://vuq.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jai.sweek.top

[E21] 超长截断加省略号
来源：http://hyb.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rpf.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nuk.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvp.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hdt.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ozn.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://iae.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ugl.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zkb.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://pgr.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ovb.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yfl.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vby.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vqb.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yds.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://coe.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://sep.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://htz.shangyingyoupin.top

================================================================================
来源：http://vem.hfpthk.cn

F. 文件与目录
来源：http://pok.0kj1m.cn

================================================================================
来源：http://uej.jinqigfzy.top

[F01] 读取整个文件
来源：http://ety.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fkd.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://qlb.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kri.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tqz.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dbf.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://igw.ybcxt.top

Ruby: File.read("a.txt")
来源：http://fzt.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://mpa.jiagoushi.top

[F02] 逐行读取文件
来源：http://imp.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tts.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gwo.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnk.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wco.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kxw.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tsl.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tfr.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zll.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://igp.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://you.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://awo.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uoh.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eav.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zlo.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dxu.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://rvo.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nzw.iojbl.cn

[F04] 追加写入文件
来源：http://itb.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hnv.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://axc.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jjr.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kko.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iwx.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uch.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qpy.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wkk.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://fxb.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hyy.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://dvn.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://kgy.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://gvb.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zpr.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zko.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://wuv.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://mik.zhijiandao.cn

[F06] 删除文件
来源：http://mfz.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://nsi.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://ckq.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://kuq.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ezs.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tqa.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://izb.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://ink.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://eup.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://oop.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sqf.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://okv.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://huo.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iua.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jpm.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mmf.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ayw.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mgv.fktsv.cn

[F08] 遍历目录
来源：http://bdm.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gus.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hke.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://wxe.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://fkg.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zxg.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dlb.ivvv.top

Ruby: Dir.children("dir")
来源：http://mau.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://djs.dashuyun.cn

[F09] 获取文件大小
来源：http://iju.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://kuo.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://ght.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://sjw.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://kxz.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jab.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qxm.nwbrower.top

Ruby: File.size("a.txt")
来源：http://rla.yangfankeji.com


<!-- 参考信息 -->