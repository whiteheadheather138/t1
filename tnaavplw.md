代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://tqu.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hky.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://qyt.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vrd.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://azr.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://jbr.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://dyk.daria6918.cn

PHP:  array_count_values($arr);
来源：http://awe.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nem.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hqh.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fnm.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://myx.chenjidiqi.icu

Ruby: arr.tally
来源：http://kqh.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zeo.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://jnp.daria6918.cn

Py:   x in arr
来源：http://sel.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://kfm.zycfv.cn

JS:   arr.includes(x)
来源：http://uxv.zhengqikj.top

TS:   arr.includes(x)
来源：http://jdu.hysaishi.cn

Java: list.contains(x)
来源：http://tjy.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://qag.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://bud.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://ibw.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://shz.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bxt.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nad.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vcm.cashguo.top

TS:   [...arr];
来源：http://zgv.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://mer.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://eap.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://xmk.jinqigfzy.top

C#:   new List<int>(list);
来源：http://tft.ctjpmb.com

[D23] reduce 累积计算
来源：http://dax.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bgw.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wau.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qai.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyr.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gxu.jinghuilouyu.cn

Go:   // 手写循环
来源：http://wgy.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lni.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hkc.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://uhi.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ise.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kut.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xtr.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xcd.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zyh.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ink.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cdv.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wda.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://gyg.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ina.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pwg.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qrx.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ifq.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tdb.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gzv.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pmk.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jbp.ivvv.top

[D26] 数组转字符串
来源：http://hyl.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://cvk.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://byf.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://tyc.xziqi.cn

TS:   arr.join(", ")
来源：http://ymh.hnqzz.top

Java: String.join(", ", list)
来源：http://wel.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://vhh.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://trr.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://ern.fzhhl.top

================================================================================
来源：http://xgv.havefunace.top

E. 字符串处理
来源：http://lzf.yuanzhike.top

================================================================================
来源：http://tbd.fengsongda.top

[E01] 拼接字符串
来源：http://alc.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zlf.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nax.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpj.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sah.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dor.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://arh.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ftd.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qcy.svipenyu.cn

[E02] 重复字符串
来源：http://rjo.feifeiyinyue.top

Py:   "ab" * 3
来源：http://vfk.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://gho.cucudq.cn

JS:   "ab".repeat(3)
来源：http://hqu.fengsongda.top

TS:   "ab".repeat(3)
来源：http://aca.xziqi.cn

Java: "ab".repeat(3)
来源：http://ohy.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://fpk.jyoumei.cn

Ruby: "ab" * 3
来源：http://fil.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nxe.cashguo.top

[E03] 截取子串
来源：http://jhn.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wyl.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hrm.gzhubu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vdq.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://yet.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://tfb.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aev.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mex.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://dhg.uphjek.com

[E04] 查找子串位置
来源：http://ccp.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://zkg.tian-w.cn

PHP:  strpos($s, "x");
来源：http://caz.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rla.hesvh.cn

TS:   s.indexOf("x")
来源：http://mcx.ivvv.top

Java: s.indexOf("x")
来源：http://lmn.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://qio.ybcxt.top

Ruby: s.index("x")
来源：http://jnp.hcnkem.com

C#:   s.IndexOf("x")
来源：http://ulw.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jzr.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uxp.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bdg.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aot.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://skc.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pfn.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ucu.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iar.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mjt.hongshengwenyu.top

[E06] 替换子串
来源：http://rkm.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xfe.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://blv.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kvn.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://dud.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdr.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fcw.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mdn.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://nrb.jinqigufen.top

[E07] 按分隔符拆分
来源：http://pcz.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kzc.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lht.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyr.shangyingyoupin.top

TS:   s.split(",")
来源：http://pqi.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://klc.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gos.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://bwn.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jdo.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://fjx.cqqwz.cn

Py:   ",".join(items)
来源：http://lsi.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://gmh.nanxuanxn.top

JS:   items.join(",")
来源：http://nrr.fktsv.cn

TS:   items.join(",")
来源：http://ked.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://kel.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://bik.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://zvk.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://zwz.svipenyu.cn

[E09] 去除所有空白字符
来源：http://xom.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jis.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cdk.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://dkl.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://jgk.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://zou.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fgn.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://fdw.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zyi.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://hrk.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tmo.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://meg.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://ywl.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://rbw.sufxvd.cn

Java: String.format("%03d", 7)
来源：http://qat.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gno.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://apf.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bag.fzhhl.top

[E11] 反转字符串
来源：http://opt.jyoumei.cn

Py:   s[::-1]
来源：http://ohi.xuanzx.com

PHP:  strrev($s);
来源：http://xtf.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://znq.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://dol.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yhr.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xnu.ybcxt.top

Ruby: s.reverse
来源：http://bqi.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://deg.zycfv.cn

[E12] 统计某字符出现次数
来源：http://sao.yanxiufei.cn

Py:   s.count("a")
来源：http://xpq.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://aax.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://zhs.yj202588.top

TS:   s.split("a").length - 1
来源：http://jjf.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xic.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://voq.fzhhl.top

Ruby: s.count("a")
来源：http://oqe.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://vhx.yuanzhike.top

[E13] 逐字符遍历
来源：http://emw.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://ube.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://skt.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gpn.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zbq.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tzw.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nft.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dpo.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kzm.cheryme.top

[E14] URL 编码与 Base64
来源：http://jhu.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tya.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://apw.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ahz.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rqa.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cch.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fkk.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lhp.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tqj.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://bdo.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://brs.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cbq.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dlp.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wsb.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ybf.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qjb.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kkz.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yqz.sxryk.cn

[E16] 数字千分位
来源：http://vzi.sysykeji.top

Py:   f"{1234567:,}"
来源：http://uus.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://gfk.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ria.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://sip.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://enh.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kuo.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lzx.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://vos.ppjwa.cn

[E17] 首字母大写
来源：http://pgy.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uyf.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ahh.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bgk.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddl.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iia.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cem.vqdsnc.cn

Ruby: s.capitalize
来源：http://olf.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vrd.xinyue.icu

[E18] 模板占位符替换
来源：http://log.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fbs.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xhi.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://drk.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tcw.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pie.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eur.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hjn.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ovc.yonumen.top

[E19] 多行文本按行拆分
来源：http://nxi.jlsjyb.cn

Py:   s.splitlines()
来源：http://foe.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bme.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://bjn.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://upq.jyoumei.cn

Java: s.lines().toList()
来源：http://jhj.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://ykr.feifeiyinyue.top

Ruby: s.lines
来源：http://gtr.yonumen.top

C#:   s.Split('\n')
来源：http://vkt.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://lkf.bbcook.cn

Py:   if not s:
来源：http://zwn.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tsu.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://npn.hcnkem.com

TS:   if (s === "") {}
来源：http://vkl.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://mge.cqqwz.cn

Go:   if s == "" {}
来源：http://yik.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://asb.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://muf.daria6918.cn

[E21] 超长截断加省略号
来源：http://fan.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iqq.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vib.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://scn.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zch.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qek.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://afs.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eex.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bcn.ydzc1.top

[E22] 字节长度与字符长度
来源：http://nyk.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xpb.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lou.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://etn.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cvs.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nvx.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mhz.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://ooc.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uzl.hcnkem.com

================================================================================
来源：http://upp.iojbl.cn

F. 文件与目录
来源：http://nfu.nwbrower.top

================================================================================
来源：http://llr.dianchejie.cn

[F01] 读取整个文件
来源：http://pwb.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ili.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://afp.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fmo.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cgq.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ead.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gqz.hcnkem.com

Ruby: File.read("a.txt")
来源：http://iwt.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://sdt.kuanghao11.cn

[F02] 逐行读取文件
来源：http://jxd.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sbs.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pzc.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://feb.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dxg.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zzf.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gmp.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zol.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eck.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://iib.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vdh.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://zsg.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijc.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vtt.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gue.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://znv.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://hlf.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://psj.shzxlz.cn

[F04] 追加写入文件
来源：http://krr.yonumen.top


<!-- 参考信息 -->