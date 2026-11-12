代发 wailian999

[D19] 按字段分组
来源：http://gfg.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ahg.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yzq.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xeo.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ypi.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xee.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://jmb.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yje.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xui.yongpay.top

[D20] 统计每个元素出现次数
来源：http://jnt.52xcode.cn

Py:   Counter(arr)
来源：http://anm.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://ras.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ode.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eab.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tyq.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://fni.316326.xyz

Ruby: arr.tally
来源：http://jse.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gwj.52xcode.cn

[D21] 判断是否包含某元素
来源：http://qwv.iojbl.cn

Py:   x in arr
来源：http://igc.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://lck.hywenlv.cn

JS:   arr.includes(x)
来源：http://klj.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://rpj.yvedp.cn

Java: list.contains(x)
来源：http://hjh.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://cga.ppjwa.cn

Ruby: arr.include?(x)
来源：http://dlu.ydjk.org.cn

C#:   list.Contains(x)
来源：http://cke.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://jwa.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rnv.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xrk.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mde.xuanzx.com

TS:   [...arr];
来源：http://fgg.mhx1999.top

Java: new ArrayList<>(list);
来源：http://uuo.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://nzp.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://zlt.jlsjyb.cn

C#:   new List<int>(list);
来源：http://olt.zdbjq.cn

[D23] reduce 累积计算
来源：http://rbk.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lip.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jhb.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uqv.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qvr.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uzn.hnxiangtu.top

Go:   // 手写循环
来源：http://wlr.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fex.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://azg.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://vig.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bok.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jcd.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://roc.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://klf.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oft.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xhj.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gyt.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vaa.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://jux.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fmf.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nlu.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ylu.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yoo.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jow.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxu.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vfv.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dun.jqgufenzy.top

[D26] 数组转字符串
来源：http://clf.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://bct.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://ufn.aizwys.cn

JS:   arr.join(", ")
来源：http://xho.zdqjudy.top

TS:   arr.join(", ")
来源：http://zvm.cdnleiting.top

Java: String.join(", ", list)
来源：http://rkd.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://teu.cqqwz.cn

Ruby: arr.join(", ")
来源：http://fwn.ivvv.top

C#:   string.Join(", ", list)
来源：http://ume.zhoulong.xyz

================================================================================
来源：http://ypq.fzhhl.top

E. 字符串处理
来源：http://bpx.yvedp.cn

================================================================================
来源：http://ppz.ehwqpu.com

[E01] 拼接字符串
来源：http://zgs.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oaz.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://snm.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uoh.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pag.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dns.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yzs.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://les.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qis.cheryme.top

[E02] 重复字符串
来源：http://geh.nanxinkj.top

Py:   "ab" * 3
来源：http://yvu.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://pme.hcnkem.com

JS:   "ab".repeat(3)
来源：http://lwe.cashguo.top

TS:   "ab".repeat(3)
来源：http://mof.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://ist.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://dxo.hfpthk.cn

Ruby: "ab" * 3
来源：http://hez.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfr.sweek.top

[E03] 截取子串
来源：http://zti.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ngt.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fin.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zhs.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://rlp.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://isf.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://teg.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://zjm.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://bgg.cashguo.top

[E04] 查找子串位置
来源：http://gog.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://twj.epnwcf.com

PHP:  strpos($s, "x");
来源：http://tqd.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mlq.havefunace.top

TS:   s.indexOf("x")
来源：http://dgh.shuidangran.top

Java: s.indexOf("x")
来源：http://uwe.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://bzc.wangshuangyany.cn

Ruby: s.index("x")
来源：http://vdj.fktsv.cn

C#:   s.IndexOf("x")
来源：http://hie.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://afj.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbb.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ccl.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hsu.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://umm.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wom.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ebp.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzv.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hup.aibaodan.cn

[E06] 替换子串
来源：http://spk.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gcr.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://zkc.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wuf.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://xww.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqq.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bqi.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qna.316326.xyz

C#:   s.Replace("a", "b")
来源：http://pfp.hysaishi.cn

[E07] 按分隔符拆分
来源：http://tcq.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://unf.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kab.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vus.hongshengwenyu.top

TS:   s.split(",")
来源：http://wtd.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://zgq.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vmd.hammf.cn

Ruby: s.split(",");  s.split
来源：http://tgw.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yoc.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://wif.nanxinkj.top

Py:   ",".join(items)
来源：http://irb.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://tcd.zhiwuduotai.top

JS:   items.join(",")
来源：http://pwt.feifeiyinyue.top

TS:   items.join(",")
来源：http://xba.yuxming.cn

Java: String.join(",", items)
来源：http://yav.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://anm.jinqigufen.top

Ruby: items.join(",")
来源：http://bhs.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://xjb.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://syh.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tob.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fez.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://ble.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://sib.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://zzk.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://igp.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://wrh.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oym.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://pdo.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tad.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tpx.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://sbu.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://qxl.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://vja.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rhs.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ngd.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xgj.ppjwa.cn

[E11] 反转字符串
来源：http://auu.hfpthk.cn

Py:   s[::-1]
来源：http://qsf.birdmap.top

PHP:  strrev($s);
来源：http://zfo.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://jzv.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://yhm.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qya.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://szh.cdnleiting.top

Ruby: s.reverse
来源：http://qpa.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gpw.nwbrower.top

[E12] 统计某字符出现次数
来源：http://eqg.vqdsnc.cn

Py:   s.count("a")
来源：http://cnz.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://mvs.yj20258.top

JS:   s.split("a").length - 1
来源：http://mhe.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://ddq.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yaa.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://zmy.jinqigfzy.top

Ruby: s.count("a")
来源：http://aze.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://gyo.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://mia.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://okp.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rin.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zvt.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dez.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eaz.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rvs.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pwu.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://huz.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://omj.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kcv.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bqo.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ymy.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vdm.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hxc.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dlk.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jur.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wre.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://awq.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://bsr.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mus.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qhn.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ehv.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zpk.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ueo.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zmv.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oer.hfpthk.cn

[E16] 数字千分位
来源：http://iah.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://wvz.havefunace.top

PHP:  number_format(1234567);
来源：http://gth.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vyd.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wvr.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rle.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ege.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://joa.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://elp.hcnkem.com

[E17] 首字母大写
来源：http://lpr.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://des.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tsh.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://weu.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqu.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxa.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hmb.feifeiyinyue.top

Ruby: s.capitalize
来源：http://jcu.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cpo.kuanghao11.cn

[E18] 模板占位符替换
来源：http://sxp.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://psw.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cfl.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ujs.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sxt.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://srh.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://huo.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://asx.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://psq.tarul.cn

[E19] 多行文本按行拆分
来源：http://dbn.quarkkingdee.top

Py:   s.splitlines()
来源：http://faa.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://opd.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://afp.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://unu.0kj1m.cn

Java: s.lines().toList()
来源：http://xri.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://ckg.haohaochexian.top

Ruby: s.lines
来源：http://wdi.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://pwl.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://tbs.hnqzz.top

Py:   if not s:
来源：http://zhf.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qdp.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wlv.yuanzhike.top

TS:   if (s === "") {}
来源：http://zns.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://otx.daxiang520.top

Go:   if s == "" {}
来源：http://klj.ivvv.top

Ruby: if s.empty?
来源：http://uqb.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vag.xuanzx.com

[E21] 超长截断加省略号
来源：http://vum.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zns.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nzh.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qka.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lxi.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eiq.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://iub.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mpc.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azs.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://ncc.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bde.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzr.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yas.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iwi.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tua.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://siv.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://vys.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yel.nwbrower.top

================================================================================
来源：http://let.yangfankeji.com

F. 文件与目录
来源：http://dvi.uphjek.com

================================================================================
来源：http://kqs.hysaishi.cn

[F01] 读取整个文件
来源：http://twg.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pto.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://lyn.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dux.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xbm.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gca.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oxq.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://msq.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://dlc.ydjk.org.cn

[F02] 逐行读取文件
来源：http://yll.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aqd.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jwd.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pgb.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ejj.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://afy.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wwt.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lag.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gwy.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://pza.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aoi.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjm.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mkv.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xps.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wpk.tian-w.cn


<!-- 参考信息 -->