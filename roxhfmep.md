代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://ltg.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jyr.uphjek.com

Go:   // 手写 map[string][]T
来源：http://zrv.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqp.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://afp.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://azv.yj20258888.top

Py:   Counter(arr)
来源：http://rua.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://miy.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://slq.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rga.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cpj.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://kro.xuetiantiany.cn

Ruby: arr.tally
来源：http://wfs.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://twl.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://buw.gotoacloud.top

Py:   x in arr
来源：http://xbl.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://lbn.mhx1999.top

JS:   arr.includes(x)
来源：http://hge.zhengqikj.top

TS:   arr.includes(x)
来源：http://kik.shuidangran.top

Java: list.contains(x)
来源：http://zen.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://iix.iojbl.cn

Ruby: arr.include?(x)
来源：http://oup.kuanghao11.cn

C#:   list.Contains(x)
来源：http://ejg.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://iqq.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ypq.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ywe.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uxr.hnqzz.top

TS:   [...arr];
来源：http://ekk.bbcook.cn

Java: new ArrayList<>(list);
来源：http://fgq.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://hiz.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://lrl.guowangkeji.top

C#:   new List<int>(list);
来源：http://asd.nanxuanxn.top

[D23] reduce 累积计算
来源：http://myp.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jop.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lsc.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hyp.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nue.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nzy.chenlongwang.top

Go:   // 手写循环
来源：http://eyt.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qob.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://anf.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://nto.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hgl.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gwk.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ofu.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vtg.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oog.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkg.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mcl.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sdp.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://ndj.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tah.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xqh.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vum.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vwr.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hvd.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zks.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nok.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jwt.quarkkingdee.top

[D26] 数组转字符串
来源：http://fhs.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://rsu.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://lbn.zdqjudy.top

JS:   arr.join(", ")
来源：http://rll.meibo888.top

TS:   arr.join(", ")
来源：http://zgv.tanke756.top

Java: String.join(", ", list)
来源：http://din.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://uuf.hnqzz.top

Ruby: arr.join(", ")
来源：http://qro.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://eni.zdbjq.cn

================================================================================
来源：http://oph.iojbl.cn

E. 字符串处理
来源：http://vfd.shanyushiyangtech.top

================================================================================
来源：http://wqu.chenjidiqi.icu

[E01] 拼接字符串
来源：http://mrz.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rdc.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kbk.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://whf.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxb.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kjk.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tmn.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qwo.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hpg.jinqigfzy.top

[E02] 重复字符串
来源：http://pna.hfpthk.cn

Py:   "ab" * 3
来源：http://agj.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://ngt.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://guq.52xcode.cn

TS:   "ab".repeat(3)
来源：http://dwg.meibo888.top

Java: "ab".repeat(3)
来源：http://jis.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://shs.cheryme.top

Ruby: "ab" * 3
来源：http://bhb.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zca.ivvv.top

[E03] 截取子串
来源：http://djz.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gik.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://azd.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ttf.sweek.top

TS:   s.slice(1, 4)
来源：http://agp.hesvh.cn

Java: s.substring(1, 4)
来源：http://diq.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://glz.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wge.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://nnk.xziqi.cn

[E04] 查找子串位置
来源：http://sfx.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://vuk.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://hip.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nmw.hnqzz.top

TS:   s.indexOf("x")
来源：http://fsz.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://fof.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://ceo.nanxinkj.top

Ruby: s.index("x")
来源：http://mud.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://mfs.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rnr.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tpj.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zgn.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvd.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://wmj.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://loi.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bxl.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eid.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vwd.fanxiaobao.xyz

[E06] 替换子串
来源：http://tcq.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eab.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://ezi.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgg.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://mgs.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgd.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyb.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sjv.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://ggn.sxryk.cn

[E07] 按分隔符拆分
来源：http://crw.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ipj.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gfc.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cjj.xuetiantiany.cn

TS:   s.split(",")
来源：http://mwb.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uzb.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://skq.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://pqz.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://chj.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://qik.sufxvd.cn

Py:   ",".join(items)
来源：http://kau.yvedp.cn

PHP:  implode(",", $items);
来源：http://zqe.gaohongyu789.top

JS:   items.join(",")
来源：http://liu.iojbl.cn

TS:   items.join(",")
来源：http://tod.daxiang520.top

Java: String.join(",", items)
来源：http://bmd.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://lpy.dianchejie.cn

Ruby: items.join(",")
来源：http://fxf.jyoumei.cn

C#:   string.Join(",", items)
来源：http://lvn.kuanghao11.cn

[E09] 去除所有空白字符
来源：http://pbw.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dxg.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rov.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://fak.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://keq.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://nyg.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mpx.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://mcv.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oxb.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://vsa.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cru.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wnp.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://gbk.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://zga.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://lhe.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yfx.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ybx.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rqk.xinyue.icu

[E11] 反转字符串
来源：http://gty.jinghuilouyu.cn

Py:   s[::-1]
来源：http://sdq.xylfe.cn

PHP:  strrev($s);
来源：http://djn.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://xah.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://ewd.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rea.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nuw.bjfxy.top

Ruby: s.reverse
来源：http://bku.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://cki.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://rnn.mhx1999.top

Py:   s.count("a")
来源：http://exn.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://xsc.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://vaj.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://wku.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uld.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://tdr.sjlbkw.cn

Ruby: s.count("a")
来源：http://mcc.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://srp.ivvv.top

[E13] 逐字符遍历
来源：http://xdy.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://gby.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zjn.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bfx.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ejw.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zbz.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yde.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sny.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://orm.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://oee.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mjp.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kwg.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ewz.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ncg.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vfs.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rcn.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aur.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jwn.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://pxr.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bho.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dqq.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lge.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sug.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xta.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fji.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lqp.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lnk.tianlin.xyz

[E16] 数字千分位
来源：http://byx.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://oaf.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://god.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://kpw.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rgp.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zjq.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://stt.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kut.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://ble.zdbjq.cn

[E17] 首字母大写
来源：http://fpr.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lbf.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bkk.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yvk.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zeu.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wzx.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://shw.316326.xyz

Ruby: s.capitalize
来源：http://gua.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ndz.yj20258.top

[E18] 模板占位符替换
来源：http://mko.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jby.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mqk.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iez.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eop.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qvc.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rcu.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dne.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://taf.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://gdj.snrcjt.cn

Py:   s.splitlines()
来源：http://hlu.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dah.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://xiw.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://mut.jiagoushi.top

Java: s.lines().toList()
来源：http://zym.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://ypq.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://tuy.kuanghao11.cn

C#:   s.Split('\n')
来源：http://myw.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://aem.cdnleiting.top

Py:   if not s:
来源：http://pty.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xma.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://epc.shanyushiyangkeji.top

TS:   if (s === "") {}
来源：http://hty.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://jyz.aizwys.cn

Go:   if s == "" {}
来源：http://mwe.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://lil.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cwo.nanxinkj.top

[E21] 超长截断加省略号
来源：http://rey.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lgk.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xal.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afw.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://opq.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pif.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://yyd.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fyd.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bwx.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://ecg.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xhj.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vbo.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hap.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cev.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lbk.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vck.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://ehc.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zxt.havefunace.top

================================================================================
来源：http://olz.yueranfly.top

F. 文件与目录
来源：http://iya.fanxiaobao.xyz

================================================================================
来源：http://tga.fzhhl.top

[F01] 读取整个文件
来源：http://mpw.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wpr.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://dye.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wkg.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zrj.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vls.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mji.zycfv.cn

Ruby: File.read("a.txt")
来源：http://odo.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://jgg.cheryme.top

[F02] 逐行读取文件
来源：http://srk.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://okf.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zya.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jbd.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qag.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ewe.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vcw.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fbr.c1oappe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ybw.pycfn.com

[F03] 写入文件（覆盖）
来源：http://ezz.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hhw.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yac.0kj1m.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oir.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oah.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://owg.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lxc.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://liw.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kgq.ydjk.org.cn

[F04] 追加写入文件
来源：http://vim.vehdjk.com


<!-- 参考信息 -->