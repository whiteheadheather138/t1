代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jbi.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yps.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kjy.yonumen.top

TS:   [...arr];
来源：http://rqr.tarul.cn

Java: new ArrayList<>(list);
来源：http://tlk.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://mgg.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://ayu.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://pqy.ppjwa.cn

[D23] reduce 累积计算
来源：http://dze.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqx.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oya.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mly.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hjl.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kka.zhoulong.xyz

Go:   // 手写循环
来源：http://mga.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tyf.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tce.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://tzn.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://req.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bqw.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vwq.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hhw.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oos.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sbo.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nse.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sps.yj20258.top

[D25] Set 集合去重与交并差
来源：http://sxw.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kut.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dwh.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qfu.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ghw.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://djq.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dro.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://arf.hesvh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mdf.zdqjudy.top

[D26] 数组转字符串
来源：http://aql.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://iyo.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://gbn.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://emr.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://tyo.zycfv.cn

Java: String.join(", ", list)
来源：http://wrs.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://ava.sysykeji.top

Ruby: arr.join(", ")
来源：http://omz.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://tjp.sweek.top

================================================================================
来源：http://ztz.cqqwz.cn

E. 字符串处理
来源：http://xfa.gzhubu.top

================================================================================
来源：http://oly.vehdjk.com

[E01] 拼接字符串
来源：http://bwc.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ahj.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gvp.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gxn.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ooa.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fdf.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vxi.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rxx.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jlg.guowangkeji.top

[E02] 重复字符串
来源：http://eqt.dashuyun.cn

Py:   "ab" * 3
来源：http://olj.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://bgg.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://trq.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://aey.vehdjk.com

Java: "ab".repeat(3)
来源：http://ndh.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://tqk.ybcxt.top

Ruby: "ab" * 3
来源：http://qwh.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fuj.hnqzz.top

[E03] 截取子串
来源：http://gvl.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kfy.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dca.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://llf.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://sgl.hywenlv.cn

Java: s.substring(1, 4)
来源：http://ygg.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lvu.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ufx.yongpay.top

C#:   s.Substring(1, 3)
来源：http://uuq.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://nan.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://qkd.hammf.cn

PHP:  strpos($s, "x");
来源：http://zfa.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gsq.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://exi.yangfankeji.com

Java: s.indexOf("x")
来源：http://waz.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://lmk.gaohongyu789.top

Ruby: s.index("x")
来源：http://eyc.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://cpb.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bhn.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wbb.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://twu.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ibr.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zgo.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lzr.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pgg.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gzj.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jlv.zhiwuduotai.top

[E06] 替换子串
来源：http://uri.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qjy.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://nvy.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cay.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://ixs.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uim.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wdu.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xdb.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://qfc.iojbl.cn

[E07] 按分隔符拆分
来源：http://rmv.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mog.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wlw.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hhf.yonumen.top

TS:   s.split(",")
来源：http://pft.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://kad.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lzy.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://eqk.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bua.hesvh.cn

[E08] 数组按分隔符合并
来源：http://ctn.daria6918.cn

Py:   ",".join(items)
来源：http://slv.tanke756.top

PHP:  implode(",", $items);
来源：http://osc.fengsongda.top

JS:   items.join(",")
来源：http://jdj.ehwqpu.com

TS:   items.join(",")
来源：http://jma.havefunace.top

Java: String.join(",", items)
来源：http://ozk.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://wlw.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://wtc.yj20258888.top

C#:   string.Join(",", items)
来源：http://lal.daria6918.cn

[E09] 去除所有空白字符
来源：http://vzs.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mvh.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eiv.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://wxf.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://riv.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://yfk.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xnd.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://bgn.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yuk.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://rmo.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ktz.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zyn.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://svb.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://jvu.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://zwv.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://stz.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kpq.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://koy.tanke756.top

[E11] 反转字符串
来源：http://khi.xuanzx.com

Py:   s[::-1]
来源：http://qai.jinqigufen.top

PHP:  strrev($s);
来源：http://qwt.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://qjx.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://wbt.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://nxc.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhx.cdnleiting.top

Ruby: s.reverse
来源：http://fga.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gzb.bbcook.cn

[E12] 统计某字符出现次数
来源：http://kkp.hywenlv.cn

Py:   s.count("a")
来源：http://tpn.tarul.cn

PHP:  substr_count($s, "a");
来源：http://fcs.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://ped.xziqi.cn

TS:   s.split("a").length - 1
来源：http://oko.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ugn.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://ubt.jinqigufen.top

Ruby: s.count("a")
来源：http://bhr.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://cix.haohaochexian.top

[E13] 逐字符遍历
来源：http://lmi.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://cez.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bjq.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tgm.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://juy.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://edo.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dhy.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://obj.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jfg.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://fye.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://taz.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohn.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tdw.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aaa.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lmp.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fmt.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://boa.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lzt.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://lom.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dhc.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yrc.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://usv.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://wgb.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lgu.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jtj.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tym.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://djo.kuanghao11.cn

[E16] 数字千分位
来源：http://qje.andypj.xyz

Py:   f"{1234567:,}"
来源：http://qvi.tanke756.top

PHP:  number_format(1234567);
来源：http://ywd.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wdt.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tqp.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ito.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uah.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://maw.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://vsf.fzhhl.top

[E17] 首字母大写
来源：http://nou.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rtb.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://zgm.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ahu.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iwt.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://muo.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tyy.jinqigfzy.top

Ruby: s.capitalize
来源：http://swa.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pih.hfpthk.cn

[E18] 模板占位符替换
来源：http://dvp.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bdi.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dxk.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zxc.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qgw.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ezq.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nsn.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vcv.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rsu.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://saf.fengsongda.top

Py:   s.splitlines()
来源：http://cgq.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vgi.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://mss.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://kmm.hesvh.cn

Java: s.lines().toList()
来源：http://fwv.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://jcc.daria6918.cn

Ruby: s.lines
来源：http://lgv.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://ihq.52xcode.cn

[E20] 判断字符串是否为空
来源：http://txx.birdmap.top

Py:   if not s:
来源：http://jwz.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kaa.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hys.xuanzx.com

TS:   if (s === "") {}
来源：http://saw.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://wmz.zhixingplan.top

Go:   if s == "" {}
来源：http://ivu.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://ikk.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xoo.ehwqpu.com

[E21] 超长截断加省略号
来源：http://rjo.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mtq.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fbp.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pog.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxq.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hua.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://mux.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vqo.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tno.yuxming.cn

[E22] 字节长度与字符长度
来源：http://mal.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yex.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddt.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://irt.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jgx.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wyv.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ush.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://hne.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lcm.fzhhl.top

================================================================================
来源：http://acx.shanyushiyangtech.top

F. 文件与目录
来源：http://fxy.hysaishi.cn

================================================================================
来源：http://aqa.chenlongwang.top

[F01] 读取整个文件
来源：http://mvg.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hrz.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://uja.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fie.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qbi.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gqp.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hhw.xinyue.icu

Ruby: File.read("a.txt")
来源：http://kmk.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://mgg.ctjpmb.com

[F02] 逐行读取文件
来源：http://cxb.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://upy.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uhq.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ghn.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjv.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yzr.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ucb.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ijj.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ucs.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://ror.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zzx.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ikl.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dlh.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cua.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fce.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://klp.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://wbd.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cqe.yuanzhike.top

[F04] 追加写入文件
来源：http://zgf.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ewg.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zam.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bcd.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iap.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rfk.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kge.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vdh.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gez.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://zcw.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rpo.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://fpv.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://btk.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://qqx.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hmv.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nza.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://uci.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://jyb.hcnkem.com

[F06] 删除文件
来源：http://vhs.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://sps.cucudq.cn

PHP:  unlink("a.txt");
来源：http://mhh.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://fjn.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://tyt.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://evp.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://xvy.zhijiandao.cn


<!-- 参考信息 -->