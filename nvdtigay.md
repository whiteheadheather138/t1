代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mvr.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rgw.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://puh.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://ozv.jqgfzy.top

Ruby: arr.tally
来源：http://uul.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://phm.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://vtt.fktsv.cn

Py:   x in arr
来源：http://nsl.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://rix.yangfankeji.com

JS:   arr.includes(x)
来源：http://fsw.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://kqe.sweek.top

Java: list.contains(x)
来源：http://rpv.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://skn.chenlongwang.top

Ruby: arr.include?(x)
来源：http://huf.zhongyouzk.top

C#:   list.Contains(x)
来源：http://mjd.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://lwd.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mbc.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qdy.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ctd.yueranfly.top

TS:   [...arr];
来源：http://sbi.meibo888.top

Java: new ArrayList<>(list);
来源：http://tgi.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://gre.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://aix.ydjk.org.cn

C#:   new List<int>(list);
来源：http://djw.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://ppa.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yxe.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zxt.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vsz.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sjz.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ftw.jiagoushi.top

Go:   // 手写循环
来源：http://hch.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xtv.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jgk.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://jpg.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vse.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://snz.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aha.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ybg.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kba.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xen.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rwy.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dkt.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://ffp.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://emc.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cpk.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://roj.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ghu.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://def.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://swn.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://snt.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xxl.jianghu66.top

[D26] 数组转字符串
来源：http://lyv.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://dbr.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://jmg.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://uyu.gogol.net.cn

TS:   arr.join(", ")
来源：http://okc.tian-w.cn

Java: String.join(", ", list)
来源：http://osf.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://lhl.epnwcf.com

Ruby: arr.join(", ")
来源：http://kjs.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://ldt.xuetiantiany.cn

================================================================================
来源：http://ait.bjfxy.top

E. 字符串处理
来源：http://uvf.uphjek.com

================================================================================
来源：http://lzs.yongpay.top

[E01] 拼接字符串
来源：http://uon.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tor.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xwv.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ltk.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://alp.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wge.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nsf.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mfz.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sap.zycfv.cn

[E02] 重复字符串
来源：http://tph.hcnkem.com

Py:   "ab" * 3
来源：http://iiv.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://ruy.iojbl.cn

JS:   "ab".repeat(3)
来源：http://yry.daria6918.cn

TS:   "ab".repeat(3)
来源：http://ges.zdbjq.cn

Java: "ab".repeat(3)
来源：http://lcs.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://pvb.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://zww.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kfj.ywan-chungtsiang.top

[E03] 截取子串
来源：http://ztb.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gzt.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://prh.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mqg.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://gmc.cashguo.top

Java: s.substring(1, 4)
来源：http://luo.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://utp.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://tud.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://bui.sweek.top

[E04] 查找子串位置
来源：http://sib.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://fzn.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://vcm.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ckn.daria6918.cn

TS:   s.indexOf("x")
来源：http://fjq.epnwcf.com

Java: s.indexOf("x")
来源：http://kzm.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://uex.tarul.cn

Ruby: s.index("x")
来源：http://zzw.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://ikn.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://eyy.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mew.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kky.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xqf.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tef.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yeg.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wwm.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pte.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lmg.zycfv.cn

[E06] 替换子串
来源：http://wqx.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rgu.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://iqi.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vyu.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://mtj.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxo.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ibu.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yog.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://svi.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://pvc.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xni.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xzj.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fda.jinqigfzy.top

TS:   s.split(",")
来源：http://hfj.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://hvq.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jjh.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://nuk.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hqo.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://rpe.dashuyun.cn

Py:   ",".join(items)
来源：http://xwl.yonumen.top

PHP:  implode(",", $items);
来源：http://ogf.vqdsnc.cn

JS:   items.join(",")
来源：http://cmw.cheryme.top

TS:   items.join(",")
来源：http://dvk.yj20258888.top

Java: String.join(",", items)
来源：http://ndr.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://fty.yj20258.top

Ruby: items.join(",")
来源：http://cre.0kj1m.cn

C#:   string.Join(",", items)
来源：http://ech.redwolf501.top

[E09] 去除所有空白字符
来源：http://zvq.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://man.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tkm.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://qqq.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://yic.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://iee.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://frf.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://cou.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zcx.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://irf.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lxs.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://etb.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://xgh.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://wtx.bbcook.cn

Java: String.format("%03d", 7)
来源：http://mbz.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://esz.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zjy.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jcc.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://ymm.0kj1m.cn

Py:   s[::-1]
来源：http://hur.zhijiandao.cn

PHP:  strrev($s);
来源：http://zas.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://unv.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://nzh.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://uew.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rlk.guannengcc.top

Ruby: s.reverse
来源：http://ple.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://eoe.cashguo.top

[E12] 统计某字符出现次数
来源：http://rcx.zhixingplan.top

Py:   s.count("a")
来源：http://afg.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://slx.yj20258888.top

JS:   s.split("a").length - 1
来源：http://onn.sysykeji.top

TS:   s.split("a").length - 1
来源：http://pko.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qho.tanke756.top

Go:   strings.Count(s, "a")
来源：http://bbc.nwbrower.top

Ruby: s.count("a")
来源：http://vfg.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://lva.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://xco.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://ybm.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jeh.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hpn.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://bpu.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://alt.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fie.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://duy.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zee.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://ljr.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://quq.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qdr.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cnx.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oib.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://unz.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pyu.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mef.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kjy.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://plw.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bvp.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ner.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vnn.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ozn.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ymf.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vzl.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bru.tianlin.xyz

[E16] 数字千分位
来源：http://eya.jianghu66.top

Py:   f"{1234567:,}"
来源：http://bqq.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://trr.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://fcs.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://ymd.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wuv.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yob.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aeu.yonumen.top

C#:   1234567.ToString("N0")
来源：http://dfy.aizwys.cn

[E17] 首字母大写
来源：http://smf.xinyue.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ijm.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://mci.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kax.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oah.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bjj.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xwq.zhongyouzk.top

Ruby: s.capitalize
来源：http://kvx.yj202588.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxt.shzxlz.cn

[E18] 模板占位符替换
来源：http://fic.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wdc.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oqh.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zok.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nhc.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fim.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nyy.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mev.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kok.ydzc1.top

[E19] 多行文本按行拆分
来源：http://zbt.quarkkingdee.top

Py:   s.splitlines()
来源：http://jwy.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lkr.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://nwg.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://ikt.jianghu66.top

Java: s.lines().toList()
来源：http://uus.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://wiu.jqgufenzy.top

Ruby: s.lines
来源：http://jxa.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://lqq.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://ztf.xylfe.cn

Py:   if not s:
来源：http://pzb.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mvc.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ual.ctjpmb.com

TS:   if (s === "") {}
来源：http://vcg.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://thu.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://aov.yuanzhike.top

Ruby: if s.empty?
来源：http://rgh.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bcp.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://bnw.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tev.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://top.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijy.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mqi.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bsc.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://vvn.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://txe.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rwz.cucudq.cn

[E22] 字节长度与字符长度
来源：http://moz.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eza.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sbn.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hlz.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mhw.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kpu.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fmv.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://rlf.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cfc.bbcook.cn

================================================================================
来源：http://zbp.zdbjq.cn

F. 文件与目录
来源：http://sgm.aibaodan.cn

================================================================================
来源：http://nqr.vqdsnc.cn

[F01] 读取整个文件
来源：http://zfz.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fek.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://vuz.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ovp.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywh.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://naa.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qsw.yueranfly.top

Ruby: File.read("a.txt")
来源：http://ese.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://jcu.cqqwz.cn

[F02] 逐行读取文件
来源：http://nwo.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ldl.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tih.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dwb.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ebh.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kna.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pbz.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pxg.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gst.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://sab.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vew.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://lso.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eyk.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bid.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jyw.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ubb.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://zbf.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rua.cheryme.top

[F04] 追加写入文件
来源：http://iru.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://urk.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mbe.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://loy.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slh.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xkq.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hjl.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://amk.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dnb.gaohongyu789.top


<!-- 参考信息 -->