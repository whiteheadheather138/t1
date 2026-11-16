代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zja.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://olf.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cfs.xuanzx.com

TS:   nested.flat();
来源：http://wsk.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oza.gzhubu.top

Go:   // 手写双层循环
来源：http://oha.ybcxt.top

Ruby: nested.flatten
来源：http://osw.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cpu.tarul.cn

[D19] 按字段分组
来源：http://uzt.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wzk.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dct.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qpo.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bpj.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gld.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://zxe.gaohongyu789.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gmz.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nih.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://nyy.xuetiantiany.cn

Py:   Counter(arr)
来源：http://yua.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://vds.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ldb.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uqf.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cxd.chenjidiqi.icu

Go:   // 手写 map[T]int
来源：http://aum.hywenlv.cn

Ruby: arr.tally
来源：http://yyk.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tfv.hcnkem.com

[D21] 判断是否包含某元素
来源：http://xtk.shangyingyoupin.top

Py:   x in arr
来源：http://utd.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://ttd.yfazqb.com

JS:   arr.includes(x)
来源：http://qmr.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://tkd.wangdashe.top

Java: list.contains(x)
来源：http://iku.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://otz.bjfxy.top

Ruby: arr.include?(x)
来源：http://ijx.aizwys.cn

C#:   list.Contains(x)
来源：http://vpp.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://tll.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qsv.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cbh.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rzy.andypj.xyz

TS:   [...arr];
来源：http://vyy.wangdashe.top

Java: new ArrayList<>(list);
来源：http://rut.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://bac.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://gwm.haohaochexian.top

C#:   new List<int>(list);
来源：http://urw.cdnleiting.top

[D23] reduce 累积计算
来源：http://ump.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lhl.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kaj.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rnu.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mbr.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xpq.shanyushiyangtech.top

Go:   // 手写循环
来源：http://uum.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yya.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://orn.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://kzj.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://exm.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sek.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://urb.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tdt.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://adx.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cyc.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ewl.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jtd.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://ieq.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ite.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rlz.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jpr.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mqj.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hyg.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nog.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ehv.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://thy.tianlin.xyz

[D26] 数组转字符串
来源：http://syt.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://gae.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://zib.meibo888.top

JS:   arr.join(", ")
来源：http://kex.fengsongda.top

TS:   arr.join(", ")
来源：http://iwl.quarkkingdee.top

Java: String.join(", ", list)
来源：http://tft.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://bls.52xcode.cn

Ruby: arr.join(", ")
来源：http://epw.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://ttv.hongshengwenyu.top

================================================================================
来源：http://cjt.cucudq.cn

E. 字符串处理
来源：http://ktz.redwolf501.top

================================================================================
来源：http://igb.epnwcf.com

[E01] 拼接字符串
来源：http://tdy.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pci.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tnx.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gal.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ikq.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xxd.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uxi.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jet.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://duo.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://cti.52xcode.cn

Py:   "ab" * 3
来源：http://gdt.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://npj.hcnkem.com

JS:   "ab".repeat(3)
来源：http://xpq.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://eav.andypj.xyz

Java: "ab".repeat(3)
来源：http://mgx.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://hiw.zycfv.cn

Ruby: "ab" * 3
来源：http://nxj.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wzi.havefunace.top

[E03] 截取子串
来源：http://vdh.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dog.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pfu.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vmt.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://xff.yfazqb.com

Java: s.substring(1, 4)
来源：http://kfw.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://llk.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://axi.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://flk.yfazqb.com

[E04] 查找子串位置
来源：http://gil.pengpengdd.cyou

Py:   s.find("x");  s.index("x")
来源：http://qvg.yongpay.top

PHP:  strpos($s, "x");
来源：http://gnl.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://juu.fengsongda.top

TS:   s.indexOf("x")
来源：http://zeo.yangfankeji.com

Java: s.indexOf("x")
来源：http://mro.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://gyg.hywenlv.cn

Ruby: s.index("x")
来源：http://ybm.yonumen.top

C#:   s.IndexOf("x")
来源：http://uen.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://uol.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kgz.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rfo.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbt.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xog.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qlo.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gej.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hpx.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eba.xuetiantiany.cn

[E06] 替换子串
来源：http://gxg.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://otq.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://yzl.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tzo.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://dvj.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brj.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oyo.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sos.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://thb.hywenlv.cn

[E07] 按分隔符拆分
来源：http://wir.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sec.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jzf.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://sjw.yongpay.top

TS:   s.split(",")
来源：http://ifn.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://huq.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nys.havefunace.top

Ruby: s.split(",");  s.split
来源：http://lvu.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://agy.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://xpb.316326.xyz

Py:   ",".join(items)
来源：http://npa.0kj1m.cn

PHP:  implode(",", $items);
来源：http://hwo.quarkkingdee.top

JS:   items.join(",")
来源：http://xgb.cdnleiting.top

TS:   items.join(",")
来源：http://onr.mhx1999.top

Java: String.join(",", items)
来源：http://hvp.birdmap.top

Go:   strings.Join(items, ",")
来源：http://bkx.feifeiyinyue.top

Ruby: items.join(",")
来源：http://vyq.chenzaomai.com

C#:   string.Join(",", items)
来源：http://dkk.hywenlv.cn

[E09] 去除所有空白字符
来源：http://tbr.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mcb.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bii.fengsongda.top

JS:   s.replace(/\s+/g, "")
来源：http://lqq.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://hww.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://koe.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://gkl.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://phd.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ime.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://enu.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://odv.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ycz.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://qrz.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://bcg.birdmap.top

Java: String.format("%03d", 7)
来源：http://sxd.jiagoushi.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wfy.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://osy.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://irv.aizwys.cn

[E11] 反转字符串
来源：http://jap.ppjwa.cn

Py:   s[::-1]
来源：http://lgr.ydzc1.top

PHP:  strrev($s);
来源：http://kvd.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://hsg.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://llo.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://plw.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://sat.shanyushiyangtech.top

Ruby: s.reverse
来源：http://grj.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gyq.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://kbb.yanxiufei.cn

Py:   s.count("a")
来源：http://das.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://kiw.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://fze.havefunace.top

TS:   s.split("a").length - 1
来源：http://ajl.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nwv.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://vdh.vehdjk.com

Ruby: s.count("a")
来源：http://rcc.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://sah.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://vpo.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://klg.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pdc.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://opf.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mrq.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gbg.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tzq.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://wsh.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cef.smart0.xyz

[E14] URL 编码与 Base64
来源：http://wvk.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xeu.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jyn.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ftk.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kvh.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yhl.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qbc.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mod.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kwt.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://nhk.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kyk.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kra.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qxn.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sii.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bpf.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://izh.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vfa.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uyn.jinghuilouyu.cn

[E16] 数字千分位
来源：http://vqm.smart0.xyz

Py:   f"{1234567:,}"
来源：http://gsy.shzxlz.cn

PHP:  number_format(1234567);
来源：http://zhs.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vdo.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xlq.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bce.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tis.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqt.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://wow.tarul.cn

[E17] 首字母大写
来源：http://epa.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dks.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://fxx.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmd.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drb.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bzu.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sgx.daria6918.cn

Ruby: s.capitalize
来源：http://ewv.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kqv.tarul.cn

[E18] 模板占位符替换
来源：http://sak.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://acy.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xwk.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nah.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://blt.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qom.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cyf.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ote.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fcb.ybcxt.top

[E19] 多行文本按行拆分
来源：http://htp.pengpengdd.cyou

Py:   s.splitlines()
来源：http://kiy.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kju.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://fkw.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://wek.wangdashe.top

Java: s.lines().toList()
来源：http://evl.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://uwz.jinqigfzy.top

Ruby: s.lines
来源：http://ngx.316326.xyz

C#:   s.Split('\n')
来源：http://ypr.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://pvv.zhoulong.xyz

Py:   if not s:
来源：http://efs.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iel.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fcd.dianchejie.cn

TS:   if (s === "") {}
来源：http://uwd.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://gnx.aizwys.cn

Go:   if s == "" {}
来源：http://xlt.redwolf501.top

Ruby: if s.empty?
来源：http://ivs.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zdl.daxiang520.top

[E21] 超长截断加省略号
来源：http://ijt.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dxh.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ddn.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyv.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lft.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jzj.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://oul.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bap.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wlb.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://qgw.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bhf.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cdw.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ixl.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uah.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://azr.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ndr.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://pgy.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ioc.hongshengwenyu.top

================================================================================
来源：http://rwi.zhaomingkeji.xyz

F. 文件与目录
来源：http://spa.yueranfly.top

================================================================================
来源：http://zoc.zdqjudy.top

[F01] 读取整个文件
来源：http://fxm.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ndi.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://nlh.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cat.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oyl.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xpa.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gur.yuxming.cn

Ruby: File.read("a.txt")
来源：http://pnf.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://hui.vqdsnc.cn

[F02] 逐行读取文件
来源：http://xzd.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xgj.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pcp.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mxh.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcn.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jrv.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bfk.yueranfly.top


<!-- 参考信息 -->