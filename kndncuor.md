代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ceb.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ycs.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jlc.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nvd.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vfp.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tsf.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://prk.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://etz.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oxa.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uez.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://frt.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pev.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ynz.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tgg.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aev.zhijiandao.cn

[D26] 数组转字符串
来源：http://sga.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://jbd.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://nmr.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://tra.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://kzi.tianlin.xyz

Java: String.join(", ", list)
来源：http://smu.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://hhc.andypj.xyz

Ruby: arr.join(", ")
来源：http://tin.fktsv.cn

C#:   string.Join(", ", list)
来源：http://qhn.svipenyu.cn

================================================================================
来源：http://ikp.zhaomingkeji.xyz

E. 字符串处理
来源：http://kqt.yj202588.top

================================================================================
来源：http://wjm.cashguo.top

[E01] 拼接字符串
来源：http://qdp.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jxz.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ruy.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kuc.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zje.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mhv.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vtn.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qep.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wxk.jianghu66.top

[E02] 重复字符串
来源：http://nka.cqqwz.cn

Py:   "ab" * 3
来源：http://mfb.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://zyl.xinyue.icu

JS:   "ab".repeat(3)
来源：http://rie.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://wtw.hywenlv.cn

Java: "ab".repeat(3)
来源：http://can.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://fan.gzhubu.top

Ruby: "ab" * 3
来源：http://atw.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lnz.jinqigufen.top

[E03] 截取子串
来源：http://gyl.aizwys.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mfk.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eiu.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://frn.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://ffx.andypj.xyz

Java: s.substring(1, 4)
来源：http://equ.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tox.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://fvj.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://amo.meibo888.top

[E04] 查找子串位置
来源：http://zyp.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://btc.meibo888.top

PHP:  strpos($s, "x");
来源：http://bqu.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://plh.cucudq.cn

TS:   s.indexOf("x")
来源：http://ylq.fehbvm.com

Java: s.indexOf("x")
来源：http://vxi.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://sun.ppjwa.cn

Ruby: s.index("x")
来源：http://rqd.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://zdq.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mpk.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://suv.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qta.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqq.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kyb.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qht.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kvo.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yog.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mlc.jinyuanbaomall.cn

[E06] 替换子串
来源：http://yig.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgz.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://drp.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://slq.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://fix.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xry.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vxv.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fum.cashguo.top

C#:   s.Replace("a", "b")
来源：http://wnq.hywenlv.cn

[E07] 按分隔符拆分
来源：http://gfj.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bay.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fsa.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gfs.jinghuilouyu.cn

TS:   s.split(",")
来源：http://ptl.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://avn.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dcq.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://rux.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gdz.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://wxb.zhongyouzk.top

Py:   ",".join(items)
来源：http://jkv.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://tay.ivvv.top

JS:   items.join(",")
来源：http://gfv.shuidangran.top

TS:   items.join(",")
来源：http://nav.wangdashe.top

Java: String.join(",", items)
来源：http://knu.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://vkb.dianchejie.cn

Ruby: items.join(",")
来源：http://ohn.sweek.top

C#:   string.Join(",", items)
来源：http://kyb.chenlongwang.top

[E09] 去除所有空白字符
来源：http://dog.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gnl.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://toj.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://nvx.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://vei.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://hdm.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kqk.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gho.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vpi.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://aig.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgk.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nay.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://fil.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://ecj.sufxvd.cn

Java: String.format("%03d", 7)
来源：http://rzh.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uqd.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rsn.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ofz.iojbl.cn

[E11] 反转字符串
来源：http://hdp.xylfe.cn

Py:   s[::-1]
来源：http://iqg.dashuyun.cn

PHP:  strrev($s);
来源：http://hrk.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://ucb.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://lnn.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://vlv.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cpp.snrcjt.cn

Ruby: s.reverse
来源：http://vff.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://nfu.zhaomingkeji.xyz

[E12] 统计某字符出现次数
来源：http://lee.jiagoushi.top

Py:   s.count("a")
来源：http://gku.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://ixi.sysykeji.top

JS:   s.split("a").length - 1
来源：http://acp.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://ahy.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qjk.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://qjs.52xcode.cn

Ruby: s.count("a")
来源：http://apz.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://akl.tian-w.cn

[E13] 逐字符遍历
来源：http://qlf.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://aia.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vqp.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://prc.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://odh.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kch.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xcj.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xmw.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tnf.cheryme.top

[E14] URL 编码与 Base64
来源：http://kmd.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mdc.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fgz.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aoo.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bbm.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nor.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wkr.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://irv.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rdo.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://uer.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xji.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kfx.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ymy.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://tgx.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jdc.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ohd.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gha.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://stk.yuanzhike.top

[E16] 数字千分位
来源：http://exc.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://odw.haohaochexian.top

PHP:  number_format(1234567);
来源：http://isz.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://upu.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wie.shuidangran.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uub.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ote.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://heg.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://ayf.shanyushiyangtech.top

[E17] 首字母大写
来源：http://qvf.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zzm.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://huv.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jyh.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hhj.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nye.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kuk.hfpthk.cn

Ruby: s.capitalize
来源：http://ndd.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xcz.daria6918.cn

[E18] 模板占位符替换
来源：http://kqg.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tgp.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qof.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://tup.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qyc.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oxq.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jps.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dpx.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://clv.tanke756.top

[E19] 多行文本按行拆分
来源：http://rws.guannengcc.top

Py:   s.splitlines()
来源：http://fqk.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jez.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://lxi.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://ion.jinqigufen.top

Java: s.lines().toList()
来源：http://zjv.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://tcu.jinqigufen.top

Ruby: s.lines
来源：http://ybs.jqgufenzy.top

C#:   s.Split('\n')
来源：http://gtu.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://fuo.guannengcc.top

Py:   if not s:
来源：http://zvv.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gch.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zbb.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://ufn.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://zkl.ydzc1.top

Go:   if s == "" {}
来源：http://cwt.zhijiandao.cn

Ruby: if s.empty?
来源：http://lau.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kmi.tarul.cn

[E21] 超长截断加省略号
来源：http://rck.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ffu.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ofv.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mku.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hky.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nbk.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://dgd.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bwi.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://amz.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://siy.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cda.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rud.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnb.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mjr.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tzq.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jgo.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://ofq.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qqu.yangfankeji.com

================================================================================
来源：http://ntq.sufxvd.cn

F. 文件与目录
来源：http://sgm.wangdashe.top

================================================================================
来源：http://jgc.andypj.xyz

[F01] 读取整个文件
来源：http://swi.c1oappe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://owj.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://gvw.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gnh.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mlh.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dkd.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jzj.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://opo.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://kmp.ehwqpu.com

[F02] 逐行读取文件
来源：http://euc.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hyb.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lpm.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rfo.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zke.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zcl.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ahr.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kxw.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgi.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://vxy.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://loa.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xaa.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fba.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://foj.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hzi.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kml.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://pso.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uak.hywenlv.cn

[F04] 追加写入文件
来源：http://lla.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uct.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dke.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bqn.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxr.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sem.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lyt.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ioo.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzf.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://cmm.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://llg.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://qhb.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://ufo.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://fun.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cvl.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hep.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://esy.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://slr.dashuyun.cn

[F06] 删除文件
来源：http://shl.cucudq.cn

Py:   os.remove("a.txt")
来源：http://haz.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://qwj.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xys.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pna.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lof.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://tjo.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://yrw.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://yjy.meibo888.top

[F07] 创建目录（含多级）
来源：http://ufo.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vgp.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mkf.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ket.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lcn.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hlc.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rjs.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qww.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hcb.ivvv.top

[F08] 遍历目录
来源：http://kgp.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zbo.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mko.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://kac.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://jvu.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eit.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://spt.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://fvb.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://guy.ivvv.top


<!-- 参考信息 -->