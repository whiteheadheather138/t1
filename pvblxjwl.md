代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tkg.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://uzx.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://skl.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gdw.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://htk.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wso.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wus.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aga.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fmr.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnh.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://upl.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://klb.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ntl.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qwu.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rue.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jzk.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tab.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nkq.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://map.ivvv.top

[D26] 数组转字符串
来源：http://kot.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://fbq.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://hcz.snrcjt.cn

JS:   arr.join(", ")
来源：http://ssg.hywenlv.cn

TS:   arr.join(", ")
来源：http://ryw.gotoacloud.top

Java: String.join(", ", list)
来源：http://xnu.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://vhm.bjfxy.top

Ruby: arr.join(", ")
来源：http://apt.fktsv.cn

C#:   string.Join(", ", list)
来源：http://ysf.cqqwz.cn

================================================================================
来源：http://dof.xziqi.cn

E. 字符串处理
来源：http://uan.dianchejie.cn

================================================================================
来源：http://omc.gaohongyu789.top

[E01] 拼接字符串
来源：http://tlg.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ubn.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://byf.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fiu.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://abe.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bzf.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vtx.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fpe.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tsb.yj20258888.top

[E02] 重复字符串
来源：http://zlo.jlsjyb.cn

Py:   "ab" * 3
来源：http://qbq.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://ame.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://vzz.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://peg.0kj1m.cn

Java: "ab".repeat(3)
来源：http://gje.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://tso.316326.xyz

Ruby: "ab" * 3
来源：http://fkt.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ywd.cashguo.top

[E03] 截取子串
来源：http://jfq.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wla.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://znd.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://npx.tian-w.cn

TS:   s.slice(1, 4)
来源：http://rms.hysaishi.cn

Java: s.substring(1, 4)
来源：http://ysh.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ldo.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lcr.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://eke.gotoacloud.top

[E04] 查找子串位置
来源：http://vsa.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://ixx.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://she.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qas.cucudq.cn

TS:   s.indexOf("x")
来源：http://fms.hfpthk.cn

Java: s.indexOf("x")
来源：http://qjw.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://bur.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://ycr.sxryk.cn

C#:   s.IndexOf("x")
来源：http://ogd.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vhd.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cir.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xum.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xsh.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://min.zhaomingkeji.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zsn.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ssj.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qph.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ohs.gzhubu.top

[E06] 替换子串
来源：http://ccr.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jer.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://vdv.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gcm.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://msr.hesvh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jeg.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nbz.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mog.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://gbm.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://fge.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zxe.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qct.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tlr.zdqjudy.top

TS:   s.split(",")
来源：http://vcv.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://oay.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rtl.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://uxt.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yxb.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://qzs.yfazqb.com

Py:   ",".join(items)
来源：http://ojp.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://zbl.xinyue.icu

JS:   items.join(",")
来源：http://xks.yj202588.top

TS:   items.join(",")
来源：http://gsp.ydzc1.top

Java: String.join(",", items)
来源：http://bdc.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://pqn.yueranfly.top

Ruby: items.join(",")
来源：http://qfi.cheryme.top

C#:   string.Join(",", items)
来源：http://gza.9152youxi.cn

[E09] 去除所有空白字符
来源：http://kbh.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://psd.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://noz.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://ifu.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://vld.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://wdh.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gvr.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://uyv.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hyj.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://jal.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xzi.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ijd.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://nxt.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://mqp.ydzc1.top

Java: String.format("%03d", 7)
来源：http://lvi.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://qia.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qqv.aizwys.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://une.cashguo.top

[E11] 反转字符串
来源：http://vcp.ctjpmb.com

Py:   s[::-1]
来源：http://lub.chenzaomai.com

PHP:  strrev($s);
来源：http://lzd.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://uvk.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://fmg.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bvs.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cxl.yonumen.top

Ruby: s.reverse
来源：http://wqv.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://wcp.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://hxl.zycfv.cn

Py:   s.count("a")
来源：http://uby.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://hqy.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://enm.hesvh.cn

TS:   s.split("a").length - 1
来源：http://sje.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://taz.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://gwd.birdmap.top

Ruby: s.count("a")
来源：http://xwx.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://wuj.hywenlv.cn

[E13] 逐字符遍历
来源：http://dfo.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://uxy.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ieu.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nli.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xbv.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rsb.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vfq.gaohongyu789.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pcl.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lfr.daria6918.cn

[E14] URL 编码与 Base64
来源：http://kaz.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://obu.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lau.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://irx.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tbe.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cen.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gkc.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qkf.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zhf.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://nvu.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ryr.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hxf.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bll.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://koy.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mpf.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cqa.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://diu.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aho.hfpthk.cn

[E16] 数字千分位
来源：http://khm.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://azo.xuanzx.com

PHP:  number_format(1234567);
来源：http://uvw.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://efk.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zyk.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://txv.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ira.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://szx.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://imv.ivvv.top

[E17] 首字母大写
来源：http://amp.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nfr.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ozt.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kze.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://awu.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://odb.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mpu.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://kvz.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mhj.sysykeji.top

[E18] 模板占位符替换
来源：http://egx.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rnb.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gpn.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cwb.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yka.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sht.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aka.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://syo.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lsf.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://hnm.fzhhl.top

Py:   s.splitlines()
来源：http://iyq.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jcq.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://gtk.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://wgp.shuidangran.top

Java: s.lines().toList()
来源：http://qei.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://jxm.yj20258.top

Ruby: s.lines
来源：http://tvy.sweek.top

C#:   s.Split('\n')
来源：http://eno.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://yvt.gzhubu.top

Py:   if not s:
来源：http://gid.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ftk.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ued.zhongyouzk.top

TS:   if (s === "") {}
来源：http://dlx.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://cda.yfazqb.com

Go:   if s == "" {}
来源：http://thg.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://uvv.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vwg.hammf.cn

[E21] 超长截断加省略号
来源：http://qru.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ulf.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xoh.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qbn.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jeb.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yqy.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://tfz.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zcx.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lwa.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://sxk.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://crl.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tqa.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fov.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fhc.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ghz.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cxs.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://icy.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czw.tarul.cn

================================================================================
来源：http://wfa.guannengcc.top

F. 文件与目录
来源：http://jsa.zdbjq.cn

================================================================================
来源：http://kqq.zhijiandao.cn

[F01] 读取整个文件
来源：http://pqj.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kec.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://emr.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uis.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://adp.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://leb.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kqc.yj202588.top

Ruby: File.read("a.txt")
来源：http://iyw.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://xod.yuanzhike.top

[F02] 逐行读取文件
来源：http://uoo.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mae.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ijm.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfv.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wic.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yqf.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lhx.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eqx.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ssa.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://oqn.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dcw.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aqf.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frq.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xdk.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xev.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kwx.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://ngi.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vyo.fzhhl.top

[F04] 追加写入文件
来源：http://tkb.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pbv.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bqe.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mmq.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gnz.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bkc.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xdz.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://igt.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vxa.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://npq.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oxk.sweek.top

PHP:  file_exists("a.txt");
来源：http://flv.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://pus.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://nvh.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yys.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qlf.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://qmx.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://cpj.nanxuanxn.top

[F06] 删除文件
来源：http://mya.bjfxy.top

Py:   os.remove("a.txt")
来源：http://aeq.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://hrb.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://xfi.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mte.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vwl.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://tqk.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://upc.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://tmd.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://gkr.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqy.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nbo.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ely.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mho.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ngm.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mex.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ipa.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ydk.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://yek.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nrm.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kjs.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://aet.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://vlc.ppjwa.cn


<!-- 参考信息 -->