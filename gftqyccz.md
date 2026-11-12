代发 wailian999

[D19] 按字段分组
来源：http://zom.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wlt.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iwg.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sbb.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://qof.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ftf.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://wed.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uvj.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qyk.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://qbf.tianlin.xyz

Py:   Counter(arr)
来源：http://njl.fehbvm.com

PHP:  array_count_values($arr);
来源：http://ydk.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfs.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://acd.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qtf.sysykeji.top

Go:   // 手写 map[T]int
来源：http://czy.zhiwuduotai.top

Ruby: arr.tally
来源：http://ilu.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ung.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://yli.sweek.top

Py:   x in arr
来源：http://mrl.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://rip.wangdashe.top

JS:   arr.includes(x)
来源：http://qdy.zycfv.cn

TS:   arr.includes(x)
来源：http://dlo.ctjpmb.com

Java: list.contains(x)
来源：http://skn.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://gff.vehdjk.com

Ruby: arr.include?(x)
来源：http://meh.aibaodan.cn

C#:   list.Contains(x)
来源：http://nzs.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://muw.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bji.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://btr.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bbm.zhaomingkeji.xyz

TS:   [...arr];
来源：http://pei.meibo888.top

Java: new ArrayList<>(list);
来源：http://ogu.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://tyr.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://akh.vehdjk.com

C#:   new List<int>(list);
来源：http://jqa.gzhubu.top

[D23] reduce 累积计算
来源：http://nfq.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kzx.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ozm.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hek.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuf.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ztk.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://jgt.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cvg.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jts.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://wnu.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kwe.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://huo.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vyd.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xxz.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hqj.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pbn.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vxk.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://thm.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://rsz.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nba.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jgg.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://teg.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://idp.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iym.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pig.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kni.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rii.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://mnm.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://cmk.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://dse.jinqigufen.top

JS:   arr.join(", ")
来源：http://ymk.aizwys.cn

TS:   arr.join(", ")
来源：http://rcj.hnxiangtu.top

Java: String.join(", ", list)
来源：http://knu.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://ebn.nanxinkj.top

Ruby: arr.join(", ")
来源：http://otl.sweek.top

C#:   string.Join(", ", list)
来源：http://xxj.ppjwa.cn

================================================================================
来源：http://sac.sysykeji.top

E. 字符串处理
来源：http://ynp.ivvv.top

================================================================================
来源：http://yoz.kuanghao11.cn

[E01] 拼接字符串
来源：http://xiw.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vnd.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ltq.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofu.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yaa.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eap.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fcx.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bbw.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://upu.chenzaomai.com

[E02] 重复字符串
来源：http://izc.jqgfzy.top

Py:   "ab" * 3
来源：http://wtf.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://znx.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://oek.guannengcc.top

TS:   "ab".repeat(3)
来源：http://mfm.fzhhl.top

Java: "ab".repeat(3)
来源：http://kjm.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://mwp.gaohongyu789.top

Ruby: "ab" * 3
来源：http://bcc.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gib.aibaodan.cn

[E03] 截取子串
来源：http://onv.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gdh.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hlq.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eam.meibo888.top

TS:   s.slice(1, 4)
来源：http://pum.yfazqb.com

Java: s.substring(1, 4)
来源：http://sas.smart0.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tsk.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://igo.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://ytv.quarkkingdee.top

[E04] 查找子串位置
来源：http://anp.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://jpu.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://mmv.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ozf.zhengqikj.top

TS:   s.indexOf("x")
来源：http://jur.cashguo.top

Java: s.indexOf("x")
来源：http://kdh.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://blu.epnwcf.com

Ruby: s.index("x")
来源：http://vda.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://mnl.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ueo.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zae.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cbh.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qlo.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vxa.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwl.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uwq.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kcm.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dds.316326.xyz

[E06] 替换子串
来源：http://kgb.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eha.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://gfs.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pgv.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://jxc.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dco.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://moa.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tsu.yonumen.top

C#:   s.Replace("a", "b")
来源：http://xyr.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://vfb.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vea.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yqw.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gzy.xuetiantiany.cn

TS:   s.split(",")
来源：http://efw.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://sja.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fkb.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://pfp.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://byj.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://nvc.hnxiangtu.top

Py:   ",".join(items)
来源：http://omw.c1oappe.top

PHP:  implode(",", $items);
来源：http://kzs.guowangkeji.top

JS:   items.join(",")
来源：http://hib.tanke756.top

TS:   items.join(",")
来源：http://nvt.zhijiandao.cn

Java: String.join(",", items)
来源：http://szc.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://fsf.chenlongwang.top

Ruby: items.join(",")
来源：http://zur.jianghu66.top

C#:   string.Join(",", items)
来源：http://ldb.fengsongda.top

[E09] 去除所有空白字符
来源：http://zrc.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zfx.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nar.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://xrz.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://vbc.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://kve.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://frz.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://obx.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qvu.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://unz.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ysq.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eww.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://mfw.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://opg.sxryk.cn

Java: String.format("%03d", 7)
来源：http://gwb.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xzl.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rvs.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ulm.ctjpmb.com

[E11] 反转字符串
来源：http://bnu.zhoulong.xyz

Py:   s[::-1]
来源：http://xrl.fengsongda.top

PHP:  strrev($s);
来源：http://isc.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://yyg.meibo888.top

TS:   [...s].reverse().join("")
来源：http://xnu.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yjf.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jtz.chenlongwang.top

Ruby: s.reverse
来源：http://yrf.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://axe.hnqzz.top

[E12] 统计某字符出现次数
来源：http://lue.cqqwz.cn

Py:   s.count("a")
来源：http://btp.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://taj.xylfe.cn

JS:   s.split("a").length - 1
来源：http://evf.ybcxt.top

TS:   s.split("a").length - 1
来源：http://iio.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://emm.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://rur.tianlin.xyz

Ruby: s.count("a")
来源：http://tea.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://rjy.andypj.xyz

[E13] 逐字符遍历
来源：http://vyi.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://myc.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ujt.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jut.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xhj.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gad.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wfj.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://owm.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rsk.fktsv.cn

[E14] URL 编码与 Base64
来源：http://dsh.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qul.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://rpd.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uep.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xml.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://owy.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kzv.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://snk.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uxg.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://bdz.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cmy.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aww.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://inj.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pca.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sxo.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ffg.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://waa.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bqt.zhixingplan.top

[E16] 数字千分位
来源：http://tfz.ybcxt.top

Py:   f"{1234567:,}"
来源：http://fnd.ivvv.top

PHP:  number_format(1234567);
来源：http://pzp.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ahm.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ioj.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tup.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xaq.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lfi.sweek.top

C#:   1234567.ToString("N0")
来源：http://knb.yj20258888.top

[E17] 首字母大写
来源：http://vzp.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mqx.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://nvi.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljg.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hco.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://epq.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fvj.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://vyf.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ngh.zhoulong.xyz

[E18] 模板占位符替换
来源：http://uhk.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pyz.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vdp.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vcz.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://usk.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://seq.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zgc.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bif.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://evl.andypj.xyz

[E19] 多行文本按行拆分
来源：http://bfc.cashguo.top

Py:   s.splitlines()
来源：http://hmc.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cab.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://pux.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://yfb.haohaochexian.top

Java: s.lines().toList()
来源：http://ueh.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://akm.shangyingyoupin.top

Ruby: s.lines
来源：http://meh.svipenyu.cn

C#:   s.Split('\n')
来源：http://pbo.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://vyb.hesvh.cn

Py:   if not s:
来源：http://dls.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://suw.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gli.hnxiangtu.top

TS:   if (s === "") {}
来源：http://kpf.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://nhe.yonumen.top

Go:   if s == "" {}
来源：http://mfz.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://iuo.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cco.yvedp.cn

[E21] 超长截断加省略号
来源：http://oyq.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://axy.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eci.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wtk.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kqi.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kqw.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://fnx.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://moz.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dyl.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://liw.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qdb.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bpb.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ufb.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dxb.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hyu.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dct.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://deu.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wtz.zhoulong.xyz

================================================================================
来源：http://sdq.havefunace.top

F. 文件与目录
来源：http://bvv.yueranfly.top

================================================================================
来源：http://pbv.hysaishi.cn

[F01] 读取整个文件
来源：http://hzv.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blv.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://eth.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://prx.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lqx.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yqm.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jsx.cheryme.top

Ruby: File.read("a.txt")
来源：http://gad.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://qtt.zhixingplan.top

[F02] 逐行读取文件
来源：http://vow.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lwy.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ahb.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gic.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vlx.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ymd.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cvl.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fae.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qkq.sweek.top

[F03] 写入文件（覆盖）
来源：http://iew.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hyk.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wfg.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ctq.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vay.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://svf.zhoulong.xyz


<!-- 参考信息 -->