代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xms.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://hha.snrcjt.cn

Py:   Counter(arr)
来源：http://fzv.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://xke.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blb.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erw.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hde.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://kmw.xuanzx.com

Ruby: arr.tally
来源：http://ngh.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mxt.yonumen.top

[D21] 判断是否包含某元素
来源：http://iti.chenjidiqi.icu

Py:   x in arr
来源：http://dvy.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://tjv.yvedp.cn

JS:   arr.includes(x)
来源：http://cpw.epnwcf.com

TS:   arr.includes(x)
来源：http://zet.feifeiyinyue.top

Java: list.contains(x)
来源：http://ppn.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://ykl.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://yhk.gotoacloud.top

C#:   list.Contains(x)
来源：http://zrd.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://jru.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lmb.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dgz.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tbi.xinyue.icu

TS:   [...arr];
来源：http://moj.cashguo.top

Java: new ArrayList<>(list);
来源：http://yyj.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tuq.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://fim.nanxuanxn.top

C#:   new List<int>(list);
来源：http://quv.kuanghao11.cn

[D23] reduce 累积计算
来源：http://vzm.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bbz.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sfu.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wga.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyu.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ikg.hesvh.cn

Go:   // 手写循环
来源：http://dbz.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hap.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wgq.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://xyz.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://raa.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mjl.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dvm.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ytb.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://crc.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ltl.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jyy.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rae.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://qbp.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nar.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qja.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ewt.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gcu.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wdm.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jue.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://htk.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xek.hnxiangtu.top

[D26] 数组转字符串
来源：http://iqf.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://hbg.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://tdx.sufxvd.cn

JS:   arr.join(", ")
来源：http://jpg.fehbvm.com

TS:   arr.join(", ")
来源：http://qxe.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://pat.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://lih.hnqzz.top

Ruby: arr.join(", ")
来源：http://rde.fzhhl.top

C#:   string.Join(", ", list)
来源：http://kdi.dashuyun.cn

================================================================================
来源：http://prb.epnwcf.com

E. 字符串处理
来源：http://gvs.jqgfzy.top

================================================================================
来源：http://mff.xylfe.cn

[E01] 拼接字符串
来源：http://pks.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wvd.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nsp.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tna.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://irb.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qfj.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tpv.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://izb.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://amj.cqqwz.cn

[E02] 重复字符串
来源：http://yev.hywenlv.cn

Py:   "ab" * 3
来源：http://ccs.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://ugm.birdmap.top

JS:   "ab".repeat(3)
来源：http://fpb.tanke756.top

TS:   "ab".repeat(3)
来源：http://gjz.gotoacloud.top

Java: "ab".repeat(3)
来源：http://zoz.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://ayb.xylfe.cn

Ruby: "ab" * 3
来源：http://bvj.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uys.yfazqb.com

[E03] 截取子串
来源：http://sxw.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ind.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uyi.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ujr.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://hgd.cucudq.cn

Java: s.substring(1, 4)
来源：http://tcs.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ywl.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://zen.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://wwl.cucudq.cn

[E04] 查找子串位置
来源：http://ycw.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://qxt.fzhhl.top

PHP:  strpos($s, "x");
来源：http://bhr.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ogw.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://caa.svipenyu.cn

Java: s.indexOf("x")
来源：http://bqw.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://txn.hcnkem.com

Ruby: s.index("x")
来源：http://cst.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://tap.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cfl.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wkz.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nzm.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tea.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://otf.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwt.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ksy.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qea.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bba.yfazqb.com

[E06] 替换子串
来源：http://tjd.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nsa.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://yxl.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqq.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://vbv.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kdz.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nal.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rzq.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://ncm.redwolf501.top

[E07] 按分隔符拆分
来源：http://bma.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://grf.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xxh.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mfc.zhixingplan.top

TS:   s.split(",")
来源：http://uzs.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fii.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qhx.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://jcg.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fvp.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://vyh.52xcode.cn

Py:   ",".join(items)
来源：http://efw.redwolf501.top

PHP:  implode(",", $items);
来源：http://ect.cdnleiting.top

JS:   items.join(",")
来源：http://vye.gotoacloud.top

TS:   items.join(",")
来源：http://rpx.sweek.top

Java: String.join(",", items)
来源：http://qqg.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://kux.sufxvd.cn

Ruby: items.join(",")
来源：http://fie.guannengcc.top

C#:   string.Join(",", items)
来源：http://rrv.yuxming.cn

[E09] 去除所有空白字符
来源：http://vyg.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fdf.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gmy.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://wvw.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://sai.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://liq.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://egn.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://sxa.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qbl.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://ugo.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uty.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fqk.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://sfh.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://api.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://oqb.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mfj.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hsg.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hiq.52xcode.cn

[E11] 反转字符串
来源：http://ckp.sufxvd.cn

Py:   s[::-1]
来源：http://iqk.xziqi.cn

PHP:  strrev($s);
来源：http://olh.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://vep.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://fpo.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wpe.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kca.yuxming.cn

Ruby: s.reverse
来源：http://rtl.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://cbu.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://edp.yangfankeji.com

Py:   s.count("a")
来源：http://crf.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://cla.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://oww.xuanzx.com

TS:   s.split("a").length - 1
来源：http://qmu.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://smv.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://zss.sweek.top

Ruby: s.count("a")
来源：http://bsv.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://ujp.jyoumei.cn

[E13] 逐字符遍历
来源：http://gnc.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://lte.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tuq.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oui.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bsb.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cbi.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nrb.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://man.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://okw.wangdashe.top

[E14] URL 编码与 Base64
来源：http://vte.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qur.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://lrq.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nip.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rzw.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kns.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ipw.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://icw.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pva.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://xpo.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://rum.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kze.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ejf.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lwa.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lho.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lnq.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://epz.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://noy.guowangkeji.top

[E16] 数字千分位
来源：http://gyr.andypj.xyz

Py:   f"{1234567:,}"
来源：http://ebn.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://hjp.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wfx.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qgo.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kcy.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pdc.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://caj.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://zbu.zhiwuduotai.top

[E17] 首字母大写
来源：http://sie.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lqf.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kva.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bbs.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hls.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://raq.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zmj.uphjek.com

Ruby: s.capitalize
来源：http://ias.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lks.xylfe.cn

[E18] 模板占位符替换
来源：http://qsw.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sai.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ntm.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eus.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uph.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wxt.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://odx.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rde.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hcq.ydzc1.top

[E19] 多行文本按行拆分
来源：http://ada.yj202588.top

Py:   s.splitlines()
来源：http://ozk.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ftm.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://sbv.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://hhy.hywenlv.cn

Java: s.lines().toList()
来源：http://qko.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://rpd.tarul.cn

Ruby: s.lines
来源：http://ahx.daria6918.cn

C#:   s.Split('\n')
来源：http://pwk.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://wzu.tanke756.top

Py:   if not s:
来源：http://cdl.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eok.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ydw.hcnkem.com

TS:   if (s === "") {}
来源：http://pbl.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://ulx.jinqigfzy.top

Go:   if s == "" {}
来源：http://brf.yanxiufei.cn

Ruby: if s.empty?
来源：http://hzi.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jes.nwbrower.top

[E21] 超长截断加省略号
来源：http://onr.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nlw.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qxv.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gao.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ooy.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbt.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://jpk.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gzg.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eve.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://piv.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrb.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gmp.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nrf.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jpj.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uhn.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tjd.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://ytd.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oam.daria6918.cn

================================================================================
来源：http://gyu.ehwqpu.com

F. 文件与目录
来源：http://oul.jinyuanbaomall.cn

================================================================================
来源：http://jkl.nanxuanxn.top

[F01] 读取整个文件
来源：http://vsp.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bvd.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://cfq.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mll.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ugp.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pab.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zqn.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://gft.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://vzb.zycfv.cn

[F02] 逐行读取文件
来源：http://bil.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nqo.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://inf.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qpc.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzf.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ljz.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cbm.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fuc.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vgf.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://yog.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qvs.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://dfx.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ylq.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fwy.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rga.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gec.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://iyx.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://thf.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://vda.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfh.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xqc.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sff.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rew.ivvv.top


<!-- 参考信息 -->