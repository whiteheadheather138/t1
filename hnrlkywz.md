代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oph.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://nkp.yj20258.top

Py:   Counter(arr)
来源：http://sro.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://sue.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pny.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wwc.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wfm.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://ney.kuanghao11.cn

Ruby: arr.tally
来源：http://ygm.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dle.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://ypc.gogol.net.cn

Py:   x in arr
来源：http://nsh.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://sgs.gaohongyu789.top

JS:   arr.includes(x)
来源：http://pbk.chenzaomai.com

TS:   arr.includes(x)
来源：http://sgg.wangdashe.top

Java: list.contains(x)
来源：http://zxu.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://wdc.redwolf501.top

Ruby: arr.include?(x)
来源：http://jgl.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://ozn.birdmap.top

[D22] 复制数组（避免共享引用）
来源：http://lsj.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qky.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cjm.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bmu.xuetiantiany.cn

TS:   [...arr];
来源：http://ahd.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://xtb.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://fvg.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://uzg.fktsv.cn

C#:   new List<int>(list);
来源：http://ulf.havefunace.top

[D23] reduce 累积计算
来源：http://pnl.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ulq.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://swp.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nca.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://efq.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mzv.jinqigufen.top

Go:   // 手写循环
来源：http://nse.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tbm.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zyj.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://shf.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sfl.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gpc.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mxs.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://auy.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xqr.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jju.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tbv.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://khk.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://gng.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://klt.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bge.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zcx.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wrr.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lbp.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iuo.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xsp.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ylc.xziqi.cn

[D26] 数组转字符串
来源：http://iwm.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://ysv.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://ejl.yj20258888.top

JS:   arr.join(", ")
来源：http://sii.jqgufenzy.top

TS:   arr.join(", ")
来源：http://kni.jianghu66.top

Java: String.join(", ", list)
来源：http://air.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://dgl.redwolf501.top

Ruby: arr.join(", ")
来源：http://nol.xylfe.cn

C#:   string.Join(", ", list)
来源：http://jjc.gzhubu.top

================================================================================
来源：http://cfq.zycfv.cn

E. 字符串处理
来源：http://vdh.zhongyouzk.top

================================================================================
来源：http://bky.hammf.cn

[E01] 拼接字符串
来源：http://ybi.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ewx.jinghuilouyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qnx.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgv.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://efg.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wfk.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ycz.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://clw.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fsn.yuanzhike.top

[E02] 重复字符串
来源：http://dtp.yvedp.cn

Py:   "ab" * 3
来源：http://vjp.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://lrp.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://jfc.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://vhu.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://fqt.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://ktc.cashguo.top

Ruby: "ab" * 3
来源：http://ixz.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bcj.zhaomingkeji.xyz

[E03] 截取子串
来源：http://uht.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hve.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://knz.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lfc.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://rmh.sufxvd.cn

Java: s.substring(1, 4)
来源：http://lqe.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vuu.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://vzk.birdmap.top

C#:   s.Substring(1, 3)
来源：http://tqk.zdqjudy.top

[E04] 查找子串位置
来源：http://duy.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://yyg.fehbvm.com

PHP:  strpos($s, "x");
来源：http://sia.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lux.cashguo.top

TS:   s.indexOf("x")
来源：http://nct.ydzc1.top

Java: s.indexOf("x")
来源：http://hvu.uphjek.com

Go:   strings.Index(s, "x")
来源：http://byw.yongpay.top

Ruby: s.index("x")
来源：http://ynk.ydzc1.top

C#:   s.IndexOf("x")
来源：http://lmu.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kie.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vsj.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aoc.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://drg.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pbq.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhs.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wyn.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://omg.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xfv.tianlin.xyz

[E06] 替换子串
来源：http://sit.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hvt.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://avk.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vhk.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://agg.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xkv.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://alm.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nrj.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://ega.nwbrower.top

[E07] 按分隔符拆分
来源：http://cki.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bxc.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aus.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pru.jlsjyb.cn

TS:   s.split(",")
来源：http://acl.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://mhr.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mld.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://pvt.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xpm.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://eqm.cucudq.cn

Py:   ",".join(items)
来源：http://cgk.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://aty.guowangkeji.top

JS:   items.join(",")
来源：http://zzr.zhijiandao.cn

TS:   items.join(",")
来源：http://qwq.bbcook.cn

Java: String.join(",", items)
来源：http://zvp.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://kpw.zhixingplan.top

Ruby: items.join(",")
来源：http://lno.aibaodan.cn

C#:   string.Join(",", items)
来源：http://lby.tian-w.cn

[E09] 去除所有空白字符
来源：http://frv.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ikf.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fqk.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://puv.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://yew.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://pzf.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://uqk.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://ats.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hor.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://exp.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://toi.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sdv.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://abs.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://cdy.meibo888.top

Java: String.format("%03d", 7)
来源：http://ats.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mku.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://msf.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxu.cheryme.top

[E11] 反转字符串
来源：http://bvj.yangfankeji.com

Py:   s[::-1]
来源：http://uze.iojbl.cn

PHP:  strrev($s);
来源：http://yhy.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://zqm.yj20258.top

TS:   [...s].reverse().join("")
来源：http://jah.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uoe.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mds.xuetiantiany.cn

Ruby: s.reverse
来源：http://dvm.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://zit.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://xgn.hywenlv.cn

Py:   s.count("a")
来源：http://fxa.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://tdy.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://evv.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://kln.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pjt.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://czu.daria6918.cn

Ruby: s.count("a")
来源：http://nfo.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://ovm.ydjk.org.cn

[E13] 逐字符遍历
来源：http://esz.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://upo.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xut.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hdl.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fad.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nub.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pas.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lqh.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pob.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://puc.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bvb.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yej.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rwo.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gcn.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://spz.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cns.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://flj.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xat.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://ncx.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bmb.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pxu.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vyp.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://cvm.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yyp.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://psj.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rmm.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://azn.shangyingyoupin.top

[E16] 数字千分位
来源：http://nug.shuidangran.top

Py:   f"{1234567:,}"
来源：http://uln.xuanzx.com

PHP:  number_format(1234567);
来源：http://ohn.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uys.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://ldn.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pju.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccz.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://coi.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://fif.zycfv.cn

[E17] 首字母大写
来源：http://joo.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ubp.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ope.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwn.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kem.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vrg.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tri.jinqigfzy.top

Ruby: s.capitalize
来源：http://zit.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyy.zdqjudy.top

[E18] 模板占位符替换
来源：http://log.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rae.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hwh.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sdz.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://trw.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rfo.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xgh.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uqd.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://afk.wangdashe.top

[E19] 多行文本按行拆分
来源：http://mfc.tian-w.cn

Py:   s.splitlines()
来源：http://rxj.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://frw.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://opj.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://zmm.redwolf501.top

Java: s.lines().toList()
来源：http://pnt.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://ntb.sjlbkw.cn

Ruby: s.lines
来源：http://dal.mhx1999.top

C#:   s.Split('\n')
来源：http://fuo.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://whk.cqqwz.cn

Py:   if not s:
来源：http://xxi.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://teg.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yhj.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://rqu.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://vyf.ctjpmb.com

Go:   if s == "" {}
来源：http://jkt.wangdashe.top

Ruby: if s.empty?
来源：http://eaj.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qrk.shuidangran.top

[E21] 超长截断加省略号
来源：http://vju.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nhm.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uor.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmd.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sla.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vxr.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://apk.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bxm.snrcjt.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ojk.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://mzk.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ved.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://szk.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dpc.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqk.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tor.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xtd.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://eha.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qbo.epnwcf.com

================================================================================
来源：http://yzm.haohaochexian.top

F. 文件与目录
来源：http://tno.sysykeji.top

================================================================================
来源：http://ihd.sysykeji.top

[F01] 读取整个文件
来源：http://xhb.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wgd.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://soz.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://exj.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rlt.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ojg.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://abe.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://fue.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://ucu.yueranfly.top

[F02] 逐行读取文件
来源：http://xzx.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kfq.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vkv.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wyc.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nyr.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yyf.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fkh.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://znv.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ryh.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://nan.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kvv.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gnz.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qrf.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yyk.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bra.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://emj.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://qfi.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jum.hcnkem.com

[F04] 追加写入文件
来源：http://egw.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://faj.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jbq.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gcl.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://for.xingfuxueyuan.xyz


<!-- 参考信息 -->