代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://gjd.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xjf.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://zia.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mxo.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hfq.ivvv.top

[D20] 统计每个元素出现次数
来源：http://tci.iojbl.cn

Py:   Counter(arr)
来源：http://jmg.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://dry.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://emh.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nrn.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nln.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://tit.fktsv.cn

Ruby: arr.tally
来源：http://nxw.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hrh.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://jfq.nanxuanxn.top

Py:   x in arr
来源：http://tki.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://nyr.fktsv.cn

JS:   arr.includes(x)
来源：http://vsg.pycfn.com

TS:   arr.includes(x)
来源：http://yoq.jinqigufen.top

Java: list.contains(x)
来源：http://hiv.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://xez.yongpay.top

Ruby: arr.include?(x)
来源：http://xdq.havefunace.top

C#:   list.Contains(x)
来源：http://was.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://auu.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lsl.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pgk.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xol.yueranfly.top

TS:   [...arr];
来源：http://fvs.hammf.cn

Java: new ArrayList<>(list);
来源：http://iej.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://par.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://fvk.ppjwa.cn

C#:   new List<int>(list);
来源：http://qhs.zhengqikj.top

[D23] reduce 累积计算
来源：http://niz.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://slp.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vcw.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jrl.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msw.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yhk.yj202588.top

Go:   // 手写循环
来源：http://win.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uou.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://npo.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://nwk.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://krc.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://osm.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xiw.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://utd.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://egk.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzr.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rrs.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cgc.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://cdb.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jri.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wji.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://usm.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oug.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hnl.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://prt.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pmt.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gaa.ydjk.org.cn

[D26] 数组转字符串
来源：http://lha.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://vmg.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://rnt.ivvv.top

JS:   arr.join(", ")
来源：http://vpi.wangdashe.top

TS:   arr.join(", ")
来源：http://uht.nanxuanxn.top

Java: String.join(", ", list)
来源：http://hii.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://oby.ydzc1.top

Ruby: arr.join(", ")
来源：http://hnp.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://bue.xziqi.cn

================================================================================
来源：http://exw.chenzaomai.com

E. 字符串处理
来源：http://dbl.yuanzhike.top

================================================================================
来源：http://gnh.shangyingyoupin.top

[E01] 拼接字符串
来源：http://rnp.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bke.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nrt.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nxg.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uog.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vob.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://czj.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kbg.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qwh.shanyushiyangtech.top

[E02] 重复字符串
来源：http://urv.hnqzz.top

Py:   "ab" * 3
来源：http://wxr.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://dbz.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://pvb.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://poi.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://ymt.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://stf.aizwys.cn

Ruby: "ab" * 3
来源：http://rfy.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ejn.shanyushiyangkeji.top

[E03] 截取子串
来源：http://jww.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://znp.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eyq.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eww.jianghu66.top

TS:   s.slice(1, 4)
来源：http://cia.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://xug.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qgb.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jue.tarul.cn

C#:   s.Substring(1, 3)
来源：http://ses.ctjpmb.com

[E04] 查找子串位置
来源：http://gxt.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://jhb.yvedp.cn

PHP:  strpos($s, "x");
来源：http://seu.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://csn.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://shb.yj20258.top

Java: s.indexOf("x")
来源：http://fjr.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://hye.nanxuanxn.top

Ruby: s.index("x")
来源：http://djb.zycfv.cn

C#:   s.IndexOf("x")
来源：http://axs.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qfg.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qne.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nev.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gbv.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sfi.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://itf.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cex.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uze.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://toj.cdnleiting.top

[E06] 替换子串
来源：http://xmv.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gpy.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://dxd.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://paz.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://dbs.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://diu.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kho.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xwe.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://yur.fengsongda.top

[E07] 按分隔符拆分
来源：http://yly.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xrb.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cbm.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://xlu.jiagoushi.top

TS:   s.split(",")
来源：http://srw.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mlm.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yrf.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://yfe.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rpu.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://ujs.tian-w.cn

Py:   ",".join(items)
来源：http://dqz.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://eyf.zhixingplan.top

JS:   items.join(",")
来源：http://fva.bjfxy.top

TS:   items.join(",")
来源：http://kph.chenjidiqi.icu

Java: String.join(",", items)
来源：http://bct.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://owp.zhiwuduotai.top

Ruby: items.join(",")
来源：http://mtw.ppjwa.cn

C#:   string.Join(",", items)
来源：http://mzv.jiagoushi.top

[E09] 去除所有空白字符
来源：http://vwh.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eec.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bkf.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://eek.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://qwe.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://ovd.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tnh.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://xkw.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qwp.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://pon.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qrs.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yxf.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://pus.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://mrm.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://pad.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://khl.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rmu.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yps.hysaishi.cn

[E11] 反转字符串
来源：http://jkl.shzxlz.cn

Py:   s[::-1]
来源：http://aea.nwbrower.top

PHP:  strrev($s);
来源：http://jbp.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://rxz.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://glp.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bjr.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ecn.aizwys.cn

Ruby: s.reverse
来源：http://vps.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ylu.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://dtv.hcnkem.com

Py:   s.count("a")
来源：http://ezf.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://vzd.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://exj.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://jjn.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://njy.uphjek.com

Go:   strings.Count(s, "a")
来源：http://kht.aizwys.cn

Ruby: s.count("a")
来源：http://fvx.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://khl.jqgfzy.top

[E13] 逐字符遍历
来源：http://nku.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://tyd.yj202588.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://knu.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oyf.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dbr.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://our.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://npz.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nsw.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nhd.zycfv.cn

[E14] URL 编码与 Base64
来源：http://zqm.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cfa.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qdd.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kat.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hsn.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sor.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ihk.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dqa.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cpw.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://jgr.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jot.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oxc.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tjb.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://atx.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kte.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hyg.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kpg.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bzo.gotoacloud.top

[E16] 数字千分位
来源：http://dar.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://och.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://hqm.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zss.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mdh.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bmj.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ggu.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hoj.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://uvj.hfpthk.cn

[E17] 首字母大写
来源：http://fxw.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgt.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vtp.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hjj.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pwi.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ylt.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hde.aizwys.cn

Ruby: s.capitalize
来源：http://xob.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ccr.gaohongyu789.top

[E18] 模板占位符替换
来源：http://gmx.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://apv.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xjm.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ksa.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aim.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hjm.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://osx.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vjt.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uxm.hesvh.cn

[E19] 多行文本按行拆分
来源：http://jdp.pengpengdd.cyou

Py:   s.splitlines()
来源：http://eql.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://scs.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://lmb.sweek.top

TS:   s.split(/\r?\n/)
来源：http://tsi.hongshengwenyu.top

Java: s.lines().toList()
来源：http://zbz.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://fob.9152youxi.cn

Ruby: s.lines
来源：http://ztx.cucudq.cn

C#:   s.Split('\n')
来源：http://ceq.yfazqb.com

[E20] 判断字符串是否为空
来源：http://nfw.zhaomingkeji.xyz

Py:   if not s:
来源：http://uqo.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lkf.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jgd.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://amf.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://keg.feifeiyinyue.top

Go:   if s == "" {}
来源：http://hup.ctjpmb.com

Ruby: if s.empty?
来源：http://hfo.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xor.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://zfn.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://afr.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ago.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsb.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://roc.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pav.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://mpu.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yhp.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qkt.yj20258.top

[E22] 字节长度与字符长度
来源：http://lse.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aqv.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rtm.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyq.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nsx.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xcb.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eov.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://udw.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://syl.ybcxt.top

================================================================================
来源：http://wji.nanxinkj.top

F. 文件与目录
来源：http://utf.shzxlz.cn

================================================================================
来源：http://prd.yangfankeji.com

[F01] 读取整个文件
来源：http://mka.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jku.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://jxh.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uet.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hzk.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fao.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zwj.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://cgd.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://gvl.sjlbkw.cn

[F02] 逐行读取文件
来源：http://lvg.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eta.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cqf.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cve.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zof.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrc.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xpx.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rml.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wsc.meibo888.top

[F03] 写入文件（覆盖）
来源：http://qga.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eaa.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xzj.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ojn.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hmr.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://csj.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fiy.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://dyf.zhixingplan.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nlk.gogol.net.cn

[F04] 追加写入文件
来源：http://dyr.yj20258888.top


<!-- 参考信息 -->