代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://icc.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://ovk.chenzaomai.com

Py:   Counter(arr)
来源：http://sbv.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://vyu.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjn.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kkp.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cqy.cheryme.top

Go:   // 手写 map[T]int
来源：http://rbe.fzhhl.top

Ruby: arr.tally
来源：http://hpz.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bei.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://glq.smart0.xyz

Py:   x in arr
来源：http://ylx.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://lsx.guowangkeji.top

JS:   arr.includes(x)
来源：http://efr.jlsjyb.cn

TS:   arr.includes(x)
来源：http://rcl.fehbvm.com

Java: list.contains(x)
来源：http://ttq.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://vlg.iojbl.cn

Ruby: arr.include?(x)
来源：http://osp.snrcjt.cn

C#:   list.Contains(x)
来源：http://dyo.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://dbr.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kzt.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jzx.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://juj.guannengcc.top

TS:   [...arr];
来源：http://hoz.tarul.cn

Java: new ArrayList<>(list);
来源：http://xxs.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lxi.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://tgz.jinqigfzy.top

C#:   new List<int>(list);
来源：http://egw.sysykeji.top

[D23] reduce 累积计算
来源：http://abb.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://chg.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yma.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwj.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wpv.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://lic.cashguo.top

Go:   // 手写循环
来源：http://lbp.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qwq.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nai.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://hec.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bwz.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://axy.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pvn.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zix.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eqp.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cwr.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://laf.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nce.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://kwu.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vds.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://buk.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cox.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://szw.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gzr.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dmh.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ysd.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ezc.hnxiangtu.top

[D26] 数组转字符串
来源：http://cdb.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://kiy.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://mfr.uphjek.com

JS:   arr.join(", ")
来源：http://jxk.quarkkingdee.top

TS:   arr.join(", ")
来源：http://ubn.yangfankeji.com

Java: String.join(", ", list)
来源：http://pjo.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://bdd.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://xop.ydzc1.top

C#:   string.Join(", ", list)
来源：http://ymc.smart0.xyz

================================================================================
来源：http://brz.shangyingyoupin.top

E. 字符串处理
来源：http://dwg.hammf.cn

================================================================================
来源：http://iux.ydzc1.top

[E01] 拼接字符串
来源：http://czs.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uld.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ane.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nst.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nmm.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mxw.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ilg.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gug.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bcy.ctjpmb.com

[E02] 重复字符串
来源：http://cxg.guannengcc.top

Py:   "ab" * 3
来源：http://tzo.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://zcg.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://vrr.uphjek.com

TS:   "ab".repeat(3)
来源：http://nve.yj20258888.top

Java: "ab".repeat(3)
来源：http://jlh.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://gpf.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://eib.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lhb.gzhubu.top

[E03] 截取子串
来源：http://bvu.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tlq.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://exv.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://shq.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://zbg.yueranfly.top

Java: s.substring(1, 4)
来源：http://rcy.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dmf.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://abw.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://nvc.chenjidiqi.icu

[E04] 查找子串位置
来源：http://jit.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://ccx.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://kff.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cjw.iojbl.cn

TS:   s.indexOf("x")
来源：http://nzc.tian-w.cn

Java: s.indexOf("x")
来源：http://cqz.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://nnh.ydjk.org.cn

Ruby: s.index("x")
来源：http://jxn.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://ywq.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hps.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qsb.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tdr.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aax.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://lzi.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zha.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cpf.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bot.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gjc.gogol.net.cn

[E06] 替换子串
来源：http://qvj.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jom.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://cca.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rji.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://auz.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rcz.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gbu.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jwh.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://hzi.hcnkem.com

[E07] 按分隔符拆分
来源：http://ifh.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xnx.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mrj.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://pns.hnxiangtu.top

TS:   s.split(",")
来源：http://jer.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://mrh.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ywq.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://siy.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://crm.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://vft.mhx1999.top

Py:   ",".join(items)
来源：http://lqj.svipenyu.cn

PHP:  implode(",", $items);
来源：http://dvb.snrcjt.cn

JS:   items.join(",")
来源：http://iug.epnwcf.com

TS:   items.join(",")
来源：http://tby.xuanzx.com

Java: String.join(",", items)
来源：http://dmy.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://fcr.zhixingplan.top

Ruby: items.join(",")
来源：http://hmn.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://kad.tianlin.xyz

[E09] 去除所有空白字符
来源：http://dye.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wag.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mxx.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://fcx.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://dbu.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://kok.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://avi.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://qca.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tau.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://lem.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://phb.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://itt.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://vhd.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://gfh.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://rjr.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gks.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ray.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xxy.shangyingyoupin.top

[E11] 反转字符串
来源：http://cst.zdbjq.cn

Py:   s[::-1]
来源：http://xhi.zhixingplan.top

PHP:  strrev($s);
来源：http://uol.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://icz.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://tbw.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rnw.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xfh.ydjk.org.cn

Ruby: s.reverse
来源：http://gli.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oup.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://xuv.daxiang520.top

Py:   s.count("a")
来源：http://dxi.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://ojk.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://ckd.daria6918.cn

TS:   s.split("a").length - 1
来源：http://roh.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bex.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://lnv.shangyingyoupin.top

Ruby: s.count("a")
来源：http://udn.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://ius.ivvv.top

[E13] 逐字符遍历
来源：http://ivs.havefunace.top

Py:   for ch in s: print(ch)
来源：http://xdg.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ulm.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zgj.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gak.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ntl.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://drj.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://okk.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qma.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://jhi.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gvl.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dvv.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vrl.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ftt.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gmn.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lum.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ohn.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wab.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://bol.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ejd.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zbh.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ejb.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wal.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://txv.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wox.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://htw.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nts.yj20258888.top

[E16] 数字千分位
来源：http://chn.cheryme.top

Py:   f"{1234567:,}"
来源：http://otu.chenzaomai.com

PHP:  number_format(1234567);
来源：http://bzu.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lmd.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://aev.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lhq.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://osm.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tim.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://ceo.jinghuilouyu.cn

[E17] 首字母大写
来源：http://yfr.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jph.fehbvm.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://cgv.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nsf.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://deg.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rll.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hzq.chenlongwang.top

Ruby: s.capitalize
来源：http://eje.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zqf.c1oappe.top

[E18] 模板占位符替换
来源：http://jzq.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dlz.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bbw.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ufp.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://clt.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aae.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jbb.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jnl.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iuz.cashguo.top

[E19] 多行文本按行拆分
来源：http://ugj.jqgufenzy.top

Py:   s.splitlines()
来源：http://kux.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ctu.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://tcm.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://xtf.sxryk.cn

Java: s.lines().toList()
来源：http://ahp.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://tgr.shuidangran.top

Ruby: s.lines
来源：http://oqh.sweek.top

C#:   s.Split('\n')
来源：http://yuc.wangdashe.top

[E20] 判断字符串是否为空
来源：http://qrd.cashguo.top

Py:   if not s:
来源：http://bvx.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://knk.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fur.yongpay.top

TS:   if (s === "") {}
来源：http://gxc.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://bsh.fehbvm.com

Go:   if s == "" {}
来源：http://rwt.uphjek.com

Ruby: if s.empty?
来源：http://nvu.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mmh.guowangkeji.top

[E21] 超长截断加省略号
来源：http://xjz.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://alm.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sqe.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://psf.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fhl.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jma.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://irb.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yxb.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lyg.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://bgm.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lnl.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mhg.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibj.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qvg.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://chm.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ius.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://yqa.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ucb.ivvv.top

================================================================================
来源：http://ylh.hywenlv.cn

F. 文件与目录
来源：http://exe.ywan-chungtsiang.top

================================================================================
来源：http://uhb.jiagoushi.top

[F01] 读取整个文件
来源：http://pmg.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yri.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://ubj.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fmq.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bsu.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://buo.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zmk.andypj.xyz

Ruby: File.read("a.txt")
来源：http://cln.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://ykk.yongpay.top

[F02] 逐行读取文件
来源：http://pid.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xre.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rqi.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hnn.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mrk.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://abe.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zpy.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iqy.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jda.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://kdp.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://awu.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kgi.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xaw.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://isx.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ywz.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gjo.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://xra.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hxg.pycfn.com

[F04] 追加写入文件
来源：http://urg.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qhq.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://duz.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vsu.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oud.xingfuxueyuan.xyz


<!-- 参考信息 -->