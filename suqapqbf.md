代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pgn.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xgu.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://olw.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zxp.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dao.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hwp.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://rym.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pqy.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bpi.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://urr.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jjq.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uek.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ode.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ryp.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bch.ivvv.top

[D26] 数组转字符串
来源：http://qhc.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://wcy.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://bym.mhx1999.top

JS:   arr.join(", ")
来源：http://egp.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://kpk.aibaodan.cn

Java: String.join(", ", list)
来源：http://pnr.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://yyu.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://lpy.jianghu66.top

C#:   string.Join(", ", list)
来源：http://tii.ehwqpu.com

================================================================================
来源：http://wnp.zdqjudy.top

E. 字符串处理
来源：http://jew.meibo888.top

================================================================================
来源：http://uuq.hesvh.cn

[E01] 拼接字符串
来源：http://ckc.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yhf.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hsh.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wim.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hcq.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rtg.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ifi.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://suo.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vvs.iojbl.cn

[E02] 重复字符串
来源：http://fzm.daria6918.cn

Py:   "ab" * 3
来源：http://pyw.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://mmy.hcnkem.com

JS:   "ab".repeat(3)
来源：http://wvv.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://xag.jqgfzy.top

Java: "ab".repeat(3)
来源：http://ghi.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://ccx.zhixingplan.top

Ruby: "ab" * 3
来源：http://qac.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gax.cqqwz.cn

[E03] 截取子串
来源：http://ssh.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bjc.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fhm.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://szh.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://kve.cdnleiting.top

Java: s.substring(1, 4)
来源：http://anu.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fqw.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://cjh.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://lrr.hammf.cn

[E04] 查找子串位置
来源：http://mvy.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://xkk.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://tnc.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zfz.epnwcf.com

TS:   s.indexOf("x")
来源：http://dso.quarkkingdee.top

Java: s.indexOf("x")
来源：http://zqv.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://uvh.snrcjt.cn

Ruby: s.index("x")
来源：http://wbr.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://iem.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wgc.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cam.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dfm.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ayr.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hqh.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://flm.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gfh.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://puz.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kdd.zdqjudy.top

[E06] 替换子串
来源：http://ljp.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://acv.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://ggl.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxa.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://lky.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uil.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wgi.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://svo.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://eni.fzhhl.top

[E07] 按分隔符拆分
来源：http://lzq.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iot.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zfp.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mhr.yangfankeji.com

TS:   s.split(",")
来源：http://mqq.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://oub.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oki.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://dcg.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kie.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://jtj.uphjek.com

Py:   ",".join(items)
来源：http://rlg.hysaishi.cn

PHP:  implode(",", $items);
来源：http://crb.kuanghao11.cn

JS:   items.join(",")
来源：http://dkx.ppjwa.cn

TS:   items.join(",")
来源：http://yil.yuxming.cn

Java: String.join(",", items)
来源：http://gtv.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://oho.fktsv.cn

Ruby: items.join(",")
来源：http://sbm.bbcook.cn

C#:   string.Join(",", items)
来源：http://qax.sxryk.cn

[E09] 去除所有空白字符
来源：http://xjd.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zgv.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vim.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://cmk.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://qpk.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://uhx.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://reh.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://pvs.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://alc.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://tje.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gdg.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://foc.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://pzq.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://dyc.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://ruy.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vrs.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kmz.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hkz.ydjk.org.cn

[E11] 反转字符串
来源：http://oay.zhijiandao.cn

Py:   s[::-1]
来源：http://jjo.hammf.cn

PHP:  strrev($s);
来源：http://lvs.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://icr.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://vtn.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vxy.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://aso.gotoacloud.top

Ruby: s.reverse
来源：http://xjt.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hbe.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://bih.bjfxy.top

Py:   s.count("a")
来源：http://isw.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://nem.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://rqy.daxiang520.top

TS:   s.split("a").length - 1
来源：http://orx.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dzl.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://vnm.birdmap.top

Ruby: s.count("a")
来源：http://vlc.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://bzy.havefunace.top

[E13] 逐字符遍历
来源：http://rhy.meibo888.top

Py:   for ch in s: print(ch)
来源：http://ais.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://snu.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://wje.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://nye.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kio.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rur.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://exo.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rsu.meibo888.top

[E14] URL 编码与 Base64
来源：http://fqq.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yhj.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://evs.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hjc.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nhz.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ozf.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bxw.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sob.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hvw.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://fjl.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ufw.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ycg.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lwj.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wmu.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eov.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://noj.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://auq.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hyn.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://fpn.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://val.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://hhs.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sdo.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://alq.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://twb.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://atp.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vjq.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://qsy.yuanzhike.top

[E17] 首字母大写
来源：http://ogk.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ysc.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xzk.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tsl.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rkg.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lra.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yfg.fzhhl.top

Ruby: s.capitalize
来源：http://paj.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tjs.ppjwa.cn

[E18] 模板占位符替换
来源：http://xbx.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://btb.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ryy.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vxn.xziqi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ntk.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cqy.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pqw.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://chk.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pfx.yj202588.top

[E19] 多行文本按行拆分
来源：http://oku.yonumen.top

Py:   s.splitlines()
来源：http://zpv.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qwt.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://gnk.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://ehz.ydjk.org.cn

Java: s.lines().toList()
来源：http://nij.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://qzb.zhaomingkeji.xyz

Ruby: s.lines
来源：http://bbw.jiagoushi.top

C#:   s.Split('\n')
来源：http://dkg.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://lci.jqgufenzy.top

Py:   if not s:
来源：http://ngv.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://idz.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mwy.zhixingplan.top

TS:   if (s === "") {}
来源：http://xzd.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://yze.jinqigfzy.top

Go:   if s == "" {}
来源：http://jnw.jqgufenzy.top

Ruby: if s.empty?
来源：http://ozj.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zml.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://wzo.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kdo.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uzz.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uuv.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yuu.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ieo.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://kgn.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hgn.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wxy.smart0.xyz

[E22] 字节长度与字符长度
来源：http://wki.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cft.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vqf.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzx.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwp.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nfl.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mxl.sweek.top

Ruby: s.bytesize;  s.length
来源：http://ngc.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ubj.daxiang520.top

================================================================================
来源：http://xls.xinyue.icu

F. 文件与目录
来源：http://gry.xuetiantiany.cn

================================================================================
来源：http://ijn.tanke756.top

[F01] 读取整个文件
来源：http://its.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://woi.meibo888.top

PHP:  file_get_contents("a.txt");
来源：http://lid.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yhv.zhaomingkeji.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qdy.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rop.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ili.daria6918.cn

Ruby: File.read("a.txt")
来源：http://lnh.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://cks.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://puo.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nzg.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gxn.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zgx.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cwt.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hcs.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xlr.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gyb.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pyh.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://muo.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://edq.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pvj.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xdw.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kbe.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hhj.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iio.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://mxj.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fco.tian-w.cn

[F04] 追加写入文件
来源：http://pfd.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ilq.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://omn.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zjd.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qlj.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lzw.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://skz.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://saf.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://inl.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://xuv.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kkw.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://vfw.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://ysi.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://qhv.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ipe.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lcg.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://avj.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://gei.zhongyouzk.top

[F06] 删除文件
来源：http://krh.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://nwy.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://rws.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://rrm.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eiy.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uwy.cashguo.top

Go:   os.Remove("a.txt")
来源：http://uve.pycfn.com

Ruby: File.delete("a.txt")
来源：http://lzw.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://nei.yj202588.top

[F07] 创建目录（含多级）
来源：http://zny.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tuc.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hzv.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cnk.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mjm.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pvj.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://thr.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tfl.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mlc.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://nuc.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://dgv.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ppn.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://gtk.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://skw.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tjd.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ebf.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://xvx.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://pen.smart0.xyz


<!-- 参考信息 -->