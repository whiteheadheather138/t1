代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://crf.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fee.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://tup.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eet.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uee.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://kvp.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mor.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://prz.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tpd.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ptl.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gvs.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://esx.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vof.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ywy.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://npj.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hxo.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lwn.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fbx.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fkd.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vzj.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wfz.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://clm.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oaq.tian-w.cn

[D26] 数组转字符串
来源：http://huw.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://ujt.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://azt.fzhhl.top

JS:   arr.join(", ")
来源：http://tbf.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://liz.yonumen.top

Java: String.join(", ", list)
来源：http://yip.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://rmr.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://nrr.cashguo.top

C#:   string.Join(", ", list)
来源：http://zbc.andypj.xyz

================================================================================
来源：http://maa.xylfe.cn

E. 字符串处理
来源：http://apr.xylfe.cn

================================================================================
来源：http://ymu.yanxiufei.cn

[E01] 拼接字符串
来源：http://hki.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zoh.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://alt.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qjh.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxd.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wgh.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tkl.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rcg.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ozd.sjlbkw.cn

[E02] 重复字符串
来源：http://jpq.hnqzz.top

Py:   "ab" * 3
来源：http://qej.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://ntn.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://dds.xinyue.icu

TS:   "ab".repeat(3)
来源：http://bnm.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://mfj.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://ept.jianghu66.top

Ruby: "ab" * 3
来源：http://bnh.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pid.fktsv.cn

[E03] 截取子串
来源：http://xky.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://osh.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jrb.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cro.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://mam.hcnkem.com

Java: s.substring(1, 4)
来源：http://fyz.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wos.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zkr.tarul.cn

C#:   s.Substring(1, 3)
来源：http://tva.mhx1999.top

[E04] 查找子串位置
来源：http://sjr.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://jts.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://oen.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kzr.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://zfu.dianchejie.cn

Java: s.indexOf("x")
来源：http://por.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://knc.pengpengdd.cyou

Ruby: s.index("x")
来源：http://poq.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://kwb.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zll.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mzl.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dey.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qos.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://tau.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wre.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ojd.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yfs.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cre.gaohongyu789.top

[E06] 替换子串
来源：http://rhg.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rdm.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://wvx.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://elx.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://hzv.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbn.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rik.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mzv.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://xza.chenzaomai.com

[E07] 按分隔符拆分
来源：http://bgb.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bwn.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://whq.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jzv.cashguo.top

TS:   s.split(",")
来源：http://tck.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://idg.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gsz.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://nqa.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qen.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://roc.yj20258888.top

Py:   ",".join(items)
来源：http://aby.aizwys.cn

PHP:  implode(",", $items);
来源：http://dov.c1oappe.top

JS:   items.join(",")
来源：http://esa.yonumen.top

TS:   items.join(",")
来源：http://kwc.zdbjq.cn

Java: String.join(",", items)
来源：http://hyz.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://bij.sufxvd.cn

Ruby: items.join(",")
来源：http://rek.fengsongda.top

C#:   string.Join(",", items)
来源：http://icj.yj202588.top

[E09] 去除所有空白字符
来源：http://ovp.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jra.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wjg.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://vdi.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://nsr.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://pil.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://uaz.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ekx.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bfo.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://gti.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fep.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hlz.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://aci.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://vlv.uphjek.com

Java: String.format("%03d", 7)
来源：http://wby.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://gbz.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vcm.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nhr.smart0.xyz

[E11] 反转字符串
来源：http://gvb.cqqwz.cn

Py:   s[::-1]
来源：http://ops.birdmap.top

PHP:  strrev($s);
来源：http://vkz.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://kit.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://ofo.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hyv.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eaw.sufxvd.cn

Ruby: s.reverse
来源：http://ujg.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://gpt.bbcook.cn

[E12] 统计某字符出现次数
来源：http://dvq.pengpengdd.cyou

Py:   s.count("a")
来源：http://lyb.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://swb.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://ncx.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://koc.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ebr.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://srd.sjlbkw.cn

Ruby: s.count("a")
来源：http://wxq.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://uke.gotoacloud.top

[E13] 逐字符遍历
来源：http://tyu.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://ovk.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://znh.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hsy.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xpf.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dvi.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://csf.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dhs.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aey.fehbvm.com

[E14] URL 编码与 Base64
来源：http://uku.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lpx.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ict.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ism.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jcp.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://epf.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xnf.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbl.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dre.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://azi.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gdp.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vqn.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zor.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://aal.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gix.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kuo.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qcx.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yro.0kj1m.cn

[E16] 数字千分位
来源：http://swl.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://sxj.yueranfly.top

PHP:  number_format(1234567);
来源：http://fuk.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dws.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ckc.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qzy.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://off.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pmv.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://gzc.chenlongwang.top

[E17] 首字母大写
来源：http://ryn.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pxp.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ldx.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://brc.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbp.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bbn.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lfr.chenjidiqi.icu

Ruby: s.capitalize
来源：http://lvb.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://agk.cheryme.top

[E18] 模板占位符替换
来源：http://wrf.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fhu.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jce.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tnz.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pby.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pev.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mjo.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qjd.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mue.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://jpg.hnqzz.top

Py:   s.splitlines()
来源：http://dbq.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lhr.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://isq.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://bhh.svipenyu.cn

Java: s.lines().toList()
来源：http://mll.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://tli.ctjpmb.com

Ruby: s.lines
来源：http://ojk.ydjk.org.cn

C#:   s.Split('\n')
来源：http://qgd.andypj.xyz

[E20] 判断字符串是否为空
来源：http://rdy.mhx1999.top

Py:   if not s:
来源：http://sfu.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eny.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fss.gogol.net.cn

TS:   if (s === "") {}
来源：http://okp.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://pdk.vehdjk.com

Go:   if s == "" {}
来源：http://wkz.smart0.xyz

Ruby: if s.empty?
来源：http://kss.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cow.hammf.cn

[E21] 超长截断加省略号
来源：http://wyv.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ztr.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://puc.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vyn.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hqy.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ncu.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://oqh.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wvv.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ygt.tanke756.top

[E22] 字节长度与字符长度
来源：http://woi.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eih.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uuy.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkg.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aoq.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ajs.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wbm.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://bqk.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rsy.hnxiangtu.top

================================================================================
来源：http://rds.xuanzx.com

F. 文件与目录
来源：http://ink.cucudq.cn

================================================================================
来源：http://lju.9152youxi.cn

[F01] 读取整个文件
来源：http://vin.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://csb.kuanghao11.cn

PHP:  file_get_contents("a.txt");
来源：http://utp.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bnt.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://abv.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hgk.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rxr.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://zlp.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://gaq.9152youxi.cn

[F02] 逐行读取文件
来源：http://jrh.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ctf.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wua.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xyr.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpx.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ezf.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kqx.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vht.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://geb.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://fly.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wia.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ldr.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffw.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmt.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jvf.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nfn.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://ker.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gtx.zycfv.cn

[F04] 追加写入文件
来源：http://wom.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dmk.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gee.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xuz.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zji.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ice.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xzi.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ing.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gjr.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://xdm.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iit.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://oce.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://wje.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://aag.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hiw.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tay.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://puu.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://nik.sxryk.cn

[F06] 删除文件
来源：http://gnh.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://pmy.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://gzf.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://isx.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://wkk.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gsk.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://dwh.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://rgx.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://wvf.tanke756.top

[F07] 创建目录（含多级）
来源：http://bbq.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sup.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zqp.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihj.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmz.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nky.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hsc.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://raa.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oks.yongpay.top

[F08] 遍历目录
来源：http://jot.havefunace.top


<!-- 参考信息 -->