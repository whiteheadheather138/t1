代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iqw.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rod.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vda.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lgj.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wro.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qlb.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://ebm.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://she.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cvo.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://keq.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lap.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xub.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oyd.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vad.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wld.iojbl.cn

[D26] 数组转字符串
来源：http://azl.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://gfs.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://kkk.sjlbkw.cn

JS:   arr.join(", ")
来源：http://drf.316326.xyz

TS:   arr.join(", ")
来源：http://thg.hammf.cn

Java: String.join(", ", list)
来源：http://cbb.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://coc.gzhubu.top

Ruby: arr.join(", ")
来源：http://sfe.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://gtv.haohaochexian.top

================================================================================
来源：http://xqk.zhiwuduotai.top

E. 字符串处理
来源：http://yhn.jqgufenzy.top

================================================================================
来源：http://oug.ivvv.top

[E01] 拼接字符串
来源：http://wep.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fdb.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vgn.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzf.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://exv.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pvs.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://soi.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zyq.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rzh.daria6918.cn

[E02] 重复字符串
来源：http://rjm.mhx1999.top

Py:   "ab" * 3
来源：http://wvl.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://oga.cheryme.top

JS:   "ab".repeat(3)
来源：http://yss.vehdjk.com

TS:   "ab".repeat(3)
来源：http://czk.yuanzhike.top

Java: "ab".repeat(3)
来源：http://qsn.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://xjm.birdmap.top

Ruby: "ab" * 3
来源：http://klu.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yoh.xziqi.cn

[E03] 截取子串
来源：http://uah.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hhp.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ypu.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bed.316326.xyz

TS:   s.slice(1, 4)
来源：http://xjx.hywenlv.cn

Java: s.substring(1, 4)
来源：http://ldz.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ame.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://uar.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://jdb.iojbl.cn

[E04] 查找子串位置
来源：http://xvs.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://keg.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://fje.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://crb.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://smm.haohaochexian.top

Java: s.indexOf("x")
来源：http://uoh.birdmap.top

Go:   strings.Index(s, "x")
来源：http://gut.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://plo.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://jwe.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://knb.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jdk.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gvz.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uyi.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://yoo.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tud.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://viy.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aee.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jqo.fzhhl.top

[E06] 替换子串
来源：http://npt.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wrm.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://gpx.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nqi.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://kjq.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://elo.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lsy.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cww.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://hkx.nanxinkj.top

[E07] 按分隔符拆分
来源：http://gfc.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sce.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ijz.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bjt.zdbjq.cn

TS:   s.split(",")
来源：http://feq.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://lxl.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://shv.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://kig.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://syn.iojbl.cn

[E08] 数组按分隔符合并
来源：http://mta.xinyue.icu

Py:   ",".join(items)
来源：http://apy.c1oappe.top

PHP:  implode(",", $items);
来源：http://odf.guowangkeji.top

JS:   items.join(",")
来源：http://dvk.shangyingyoupin.top

TS:   items.join(",")
来源：http://sol.gogol.net.cn

Java: String.join(",", items)
来源：http://vwh.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://ryw.nanxinkj.top

Ruby: items.join(",")
来源：http://zoy.ctjpmb.com

C#:   string.Join(",", items)
来源：http://lnh.gzhubu.top

[E09] 去除所有空白字符
来源：http://pmd.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ewi.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ktk.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://zlm.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://mit.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://vlw.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://zjq.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://vcc.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbl.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://xlb.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ymm.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://adq.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://gnk.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://dqo.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://gtw.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rlx.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ytd.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zfd.zhongyouzk.top

[E11] 反转字符串
来源：http://ony.316326.xyz

Py:   s[::-1]
来源：http://aoo.yj20258888.top

PHP:  strrev($s);
来源：http://cbn.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://nuf.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://ltk.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hvn.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://spu.zdbjq.cn

Ruby: s.reverse
来源：http://kxb.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://vbu.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://ock.yangfankeji.com

Py:   s.count("a")
来源：http://zzy.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://ren.sxryk.cn

JS:   s.split("a").length - 1
来源：http://lnr.yongpay.top

TS:   s.split("a").length - 1
来源：http://bdg.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dfs.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://pki.fengsongda.top

Ruby: s.count("a")
来源：http://kdl.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://nnu.nanxinkj.top

[E13] 逐字符遍历
来源：http://bhx.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://jgg.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dte.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iau.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oxv.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dye.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zyg.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://eic.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rqe.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://lbw.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wbc.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wyv.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dic.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gjz.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vky.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qll.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uyy.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dyy.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://rzb.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xlr.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://plr.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pqh.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://tkb.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://loj.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sln.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cnu.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mvj.sweek.top

[E16] 数字千分位
来源：http://ztj.ydzc1.top

Py:   f"{1234567:,}"
来源：http://wvg.sxryk.cn

PHP:  number_format(1234567);
来源：http://jfe.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fbv.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sts.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cat.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cyu.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pei.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://jvx.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://rqn.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tkm.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kps.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gyq.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yhc.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rty.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bkb.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://omb.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xex.0kj1m.cn

[E18] 模板占位符替换
来源：http://vcy.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://efw.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://khe.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uqb.jinqigufen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://czc.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dha.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zdb.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wpl.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dof.wangdashe.top

[E19] 多行文本按行拆分
来源：http://fgc.gotoacloud.top

Py:   s.splitlines()
来源：http://hno.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pht.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://fch.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://xju.wangdashe.top

Java: s.lines().toList()
来源：http://mww.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://hpw.cqqwz.cn

Ruby: s.lines
来源：http://efq.dianchejie.cn

C#:   s.Split('\n')
来源：http://qjj.c1oappe.top

[E20] 判断字符串是否为空
来源：http://ksp.sweek.top

Py:   if not s:
来源：http://bbs.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ibq.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aob.hnxiangtu.top

TS:   if (s === "") {}
来源：http://nbz.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://msx.yuanzhike.top

Go:   if s == "" {}
来源：http://lyo.cheryme.top

Ruby: if s.empty?
来源：http://emq.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://djj.uphjek.com

[E21] 超长截断加省略号
来源：http://pxr.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qgq.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qga.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsn.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ore.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qos.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://gie.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zod.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://amj.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://bwt.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vca.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dan.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cza.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nfh.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cwo.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fdc.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://hhs.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qwy.52xcode.cn

================================================================================
来源：http://kqk.havefunace.top

F. 文件与目录
来源：http://knl.shangyingyoupin.top

================================================================================
来源：http://zmt.tian-w.cn

[F01] 读取整个文件
来源：http://lsn.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nlg.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://rip.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hmm.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iib.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ytc.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nev.ybcxt.top

Ruby: File.read("a.txt")
来源：http://ukr.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://syq.zdqjudy.top

[F02] 逐行读取文件
来源：http://idv.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cod.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vum.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zra.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zab.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yqj.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sut.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dla.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mnf.uphjek.com

[F03] 写入文件（覆盖）
来源：http://zxo.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://spk.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pde.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fjn.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umb.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://heh.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zdr.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://hlx.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xwe.ppjwa.cn

[F04] 追加写入文件
来源：http://cei.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xby.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vrr.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dmq.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zbv.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pin.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rvm.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fqt.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ctu.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://iyu.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bfp.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://dja.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://tit.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://qhc.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rmd.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pxg.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://tyq.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://btw.snrcjt.cn

[F06] 删除文件
来源：http://dtk.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://hpv.shuidangran.top

PHP:  unlink("a.txt");
来源：http://ocf.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://epf.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://tzd.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bie.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://baa.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://jvo.yj20258.top

C#:   File.Delete("a.txt");
来源：http://ubq.ivvv.top

[F07] 创建目录（含多级）
来源：http://bmf.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://myh.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ons.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bsu.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://esp.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ihc.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uak.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cdk.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hls.bjfxy.top

[F08] 遍历目录
来源：http://cnv.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nri.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sfo.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://qrb.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://obm.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pbr.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://noo.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://eeu.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://xvk.zhengqikj.top


<!-- 参考信息 -->