代发 wailian999

[D19] 按字段分组
来源：http://xqx.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nvw.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ikr.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qlo.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gkj.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://psw.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://spd.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://tgm.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ukz.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://drc.c1oappe.top

Py:   Counter(arr)
来源：http://wbv.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://ena.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wkk.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gkx.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://daf.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://vml.zhiwuduotai.top

Ruby: arr.tally
来源：http://flj.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ows.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://bzo.smart0.xyz

Py:   x in arr
来源：http://ukl.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://xez.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://iui.nanxinkj.top

TS:   arr.includes(x)
来源：http://uqu.vehdjk.com

Java: list.contains(x)
来源：http://gtf.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://hos.yfazqb.com

Ruby: arr.include?(x)
来源：http://udu.sxryk.cn

C#:   list.Contains(x)
来源：http://tsi.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://qdu.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vtw.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ccx.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lei.sysykeji.top

TS:   [...arr];
来源：http://hyq.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://lkx.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://vhn.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://cyv.hywenlv.cn

C#:   new List<int>(list);
来源：http://mfa.xinyue.icu

[D23] reduce 累积计算
来源：http://rdc.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gax.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://coq.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzq.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lok.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vam.chenjidiqi.icu

Go:   // 手写循环
来源：http://edm.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ehm.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kty.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://lcc.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qbf.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gsb.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ylx.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bsl.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tak.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wqr.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bul.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wph.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://pnp.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cup.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zxp.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://euo.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fht.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fav.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://niw.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mou.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xto.tian-w.cn

[D26] 数组转字符串
来源：http://mnx.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://ntr.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://noo.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://whs.quarkkingdee.top

TS:   arr.join(", ")
来源：http://jqh.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://xta.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://mex.tianlin.xyz

Ruby: arr.join(", ")
来源：http://hqq.jianghu66.top

C#:   string.Join(", ", list)
来源：http://ynl.zhongyouzk.top

================================================================================
来源：http://zuo.zhoulong.xyz

E. 字符串处理
来源：http://atc.shanyushiyangtech.top

================================================================================
来源：http://umo.xuanzx.com

[E01] 拼接字符串
来源：http://rsw.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyy.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://icy.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hax.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://whj.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lfc.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ojl.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aiy.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://efj.hcnkem.com

[E02] 重复字符串
来源：http://gel.ydjk.org.cn

Py:   "ab" * 3
来源：http://vak.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://wes.316326.xyz

JS:   "ab".repeat(3)
来源：http://bbv.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://joz.9152youxi.cn

Java: "ab".repeat(3)
来源：http://rby.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://ykk.fehbvm.com

Ruby: "ab" * 3
来源：http://bid.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uej.meibo888.top

[E03] 截取子串
来源：http://mpp.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lli.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nsl.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wqd.zycfv.cn

TS:   s.slice(1, 4)
来源：http://lhm.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://nbj.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sqv.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ioz.meibo888.top

C#:   s.Substring(1, 3)
来源：http://jef.ivvv.top

[E04] 查找子串位置
来源：http://jnc.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://umy.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://pgj.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://paq.nwbrower.top

TS:   s.indexOf("x")
来源：http://irm.yj20258888.top

Java: s.indexOf("x")
来源：http://bvj.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://fhj.shuidangran.top

Ruby: s.index("x")
来源：http://oym.ydzc1.top

C#:   s.IndexOf("x")
来源：http://ols.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hfe.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dyc.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hki.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zan.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://grw.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nxw.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jef.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://its.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tch.zhixingplan.top

[E06] 替换子串
来源：http://zih.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rtw.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://bef.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xoa.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://zsz.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qph.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yhu.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kmn.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://jqh.zhengqikj.top

[E07] 按分隔符拆分
来源：http://kpq.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oox.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://his.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://uwn.cucudq.cn

TS:   s.split(",")
来源：http://jne.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://vap.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://obv.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://izu.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://llc.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://fcn.hfpthk.cn

Py:   ",".join(items)
来源：http://flg.sweek.top

PHP:  implode(",", $items);
来源：http://gzo.daria6918.cn

JS:   items.join(",")
来源：http://maq.hammf.cn

TS:   items.join(",")
来源：http://mks.guannengcc.top

Java: String.join(",", items)
来源：http://heg.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://tef.zhengqikj.top

Ruby: items.join(",")
来源：http://wrd.tian-w.cn

C#:   string.Join(",", items)
来源：http://xoo.316326.xyz

[E09] 去除所有空白字符
来源：http://rye.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://clj.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zkr.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://qfh.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://cff.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://qnd.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://frr.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://agw.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gtf.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://rtd.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fzv.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sfr.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://gvy.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://hdg.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://ryj.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jup.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vyu.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jaq.hcnkem.com

[E11] 反转字符串
来源：http://rnk.ydjk.org.cn

Py:   s[::-1]
来源：http://yvg.zhiwuduotai.top

PHP:  strrev($s);
来源：http://tfl.meibo888.top

JS:   [...s].reverse().join("")
来源：http://ouz.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://izn.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aqp.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nng.hywenlv.cn

Ruby: s.reverse
来源：http://ihs.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://vge.sweek.top

[E12] 统计某字符出现次数
来源：http://res.ehwqpu.com

Py:   s.count("a")
来源：http://rgu.yonumen.top

PHP:  substr_count($s, "a");
来源：http://jlj.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://lsm.yj20258.top

TS:   s.split("a").length - 1
来源：http://hhe.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://veu.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://anz.guowangkeji.top

Ruby: s.count("a")
来源：http://naf.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://exv.yvedp.cn

[E13] 逐字符遍历
来源：http://ixv.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://ayq.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhg.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mpc.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://grg.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jof.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pik.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://obr.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zxa.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://epv.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vzk.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zqz.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oyc.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hqn.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yxt.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://trv.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yof.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rff.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://sss.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kwb.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uks.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sqv.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ljl.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fgo.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ebq.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mha.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dqu.andypj.xyz

[E16] 数字千分位
来源：http://tei.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://fbe.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://rlj.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://htm.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iug.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aga.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ojz.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://syl.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://lkz.cashguo.top

[E17] 首字母大写
来源：http://jsn.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vgj.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://phr.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xtn.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hqi.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://brk.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zha.gogol.net.cn

Ruby: s.capitalize
来源：http://gun.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pgj.meibo888.top

[E18] 模板占位符替换
来源：http://pdq.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://otv.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bli.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xdx.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ddu.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ped.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qxd.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mcj.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lse.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://cge.wangdashe.top

Py:   s.splitlines()
来源：http://xsz.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://unr.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://erf.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://cbq.yj20258888.top

Java: s.lines().toList()
来源：http://dwp.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://mvw.jqgufenzy.top

Ruby: s.lines
来源：http://rzs.jqgufenzy.top

C#:   s.Split('\n')
来源：http://zpg.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://pzf.tian-w.cn

Py:   if not s:
来源：http://upg.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://abi.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kly.guowangkeji.top

TS:   if (s === "") {}
来源：http://fkg.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://cpg.zhijiandao.cn

Go:   if s == "" {}
来源：http://tdw.yanxiufei.cn

Ruby: if s.empty?
来源：http://ndj.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blr.sufxvd.cn

[E21] 超长截断加省略号
来源：http://zqd.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rvs.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gwg.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tty.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lim.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wqn.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://wxg.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uwj.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ejm.fehbvm.com

[E22] 字节长度与字符长度
来源：http://pky.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ypw.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sot.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cic.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uzy.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ozq.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qpt.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://ezz.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://msk.jyoumei.cn

================================================================================
来源：http://rzr.ydjk.org.cn

F. 文件与目录
来源：http://tyg.52xcode.cn

================================================================================
来源：http://lah.smart0.xyz

[F01] 读取整个文件
来源：http://mhj.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yqb.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://hvq.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nik.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bii.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jvc.hesvh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zkc.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://tgd.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://ruu.gzhubu.top

[F02] 逐行读取文件
来源：http://lxn.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kwz.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ukm.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ofi.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://krk.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqy.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zrg.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://odf.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mjp.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://pay.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mdr.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://qoj.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gcx.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://igh.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pyb.xingfuxueyuan.xyz


<!-- 参考信息 -->