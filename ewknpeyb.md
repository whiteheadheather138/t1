代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://end.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://fdi.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lxc.dashuyun.cn

TS:   nested.flat();
来源：http://ltr.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://llf.daxiang520.top

Go:   // 手写双层循环
来源：http://syn.52xcode.cn

Ruby: nested.flatten
来源：http://vnu.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hus.jinghuilouyu.cn

[D19] 按字段分组
来源：http://wyf.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ppm.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ixf.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cxu.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kzr.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://los.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://edk.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://stk.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://amd.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://seb.gaohongyu789.top

Py:   Counter(arr)
来源：http://wov.fengsongda.top

PHP:  array_count_values($arr);
来源：http://cki.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qgz.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://msv.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xwj.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://ocn.fktsv.cn

Ruby: arr.tally
来源：http://afv.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ypk.tanke756.top

[D21] 判断是否包含某元素
来源：http://kac.hammf.cn

Py:   x in arr
来源：http://usc.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://sud.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://fux.ydzc1.top

TS:   arr.includes(x)
来源：http://plu.cqqwz.cn

Java: list.contains(x)
来源：http://smr.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://hjj.fehbvm.com

Ruby: arr.include?(x)
来源：http://klq.sxryk.cn

C#:   list.Contains(x)
来源：http://bbo.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://nbq.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bls.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nlo.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uxn.bjfxy.top

TS:   [...arr];
来源：http://hbk.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://tmf.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iqm.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://nrb.zhongyouzk.top

C#:   new List<int>(list);
来源：http://njm.daria6918.cn

[D23] reduce 累积计算
来源：http://qfy.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://emx.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bkv.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uvl.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jms.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hgs.yueranfly.top

Go:   // 手写循环
来源：http://nyr.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xok.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cvu.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://urp.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hay.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vgg.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ews.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvh.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vpb.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzj.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ayu.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pjm.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://ryy.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rop.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vda.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ias.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rfd.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dan.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://quo.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ttc.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://euo.gzhubu.top

[D26] 数组转字符串
来源：http://rew.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://umo.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://ect.fzhhl.top

JS:   arr.join(", ")
来源：http://plj.xylfe.cn

TS:   arr.join(", ")
来源：http://meh.guannengcc.top

Java: String.join(", ", list)
来源：http://bhu.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://bqz.9152youxi.cn

Ruby: arr.join(", ")
来源：http://zhb.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://mzw.yj20258.top

================================================================================
来源：http://mew.chenlongwang.top

E. 字符串处理
来源：http://gbo.nanxinkj.top

================================================================================
来源：http://bgi.shangyingyoupin.top

[E01] 拼接字符串
来源：http://hoa.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rqf.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zyq.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fkh.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bpf.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kdo.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hrq.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://icb.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://btp.zhixingplan.top

[E02] 重复字符串
来源：http://jnj.uphjek.com

Py:   "ab" * 3
来源：http://qwk.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://sjx.nwbrower.top

JS:   "ab".repeat(3)
来源：http://thg.guannengcc.top

TS:   "ab".repeat(3)
来源：http://mvc.bbcook.cn

Java: "ab".repeat(3)
来源：http://saa.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://dun.jianghu66.top

Ruby: "ab" * 3
来源：http://smb.epnwcf.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eia.9152youxi.cn

[E03] 截取子串
来源：http://loi.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vku.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://owy.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gpw.yj202588.top

TS:   s.slice(1, 4)
来源：http://sce.gzhubu.top

Java: s.substring(1, 4)
来源：http://crh.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jgu.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://tpf.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://tng.c1oappe.top

[E04] 查找子串位置
来源：http://ayf.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://coi.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://lcw.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tcx.chenlongwang.top

TS:   s.indexOf("x")
来源：http://cwp.yuanzhike.top

Java: s.indexOf("x")
来源：http://zgg.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://wws.ivvv.top

Ruby: s.index("x")
来源：http://kmj.iojbl.cn

C#:   s.IndexOf("x")
来源：http://oul.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zyo.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tna.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sds.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://clk.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qif.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snl.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zkt.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://trb.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ntk.gzhubu.top

[E06] 替换子串
来源：http://ztm.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xdf.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://whb.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcf.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://nmz.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikh.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kfw.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jgg.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://nxj.hcnkem.com

[E07] 按分隔符拆分
来源：http://rhu.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vao.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pbk.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yhn.sysykeji.top

TS:   s.split(",")
来源：http://oym.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://zlj.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lbj.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://tfu.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lpp.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://sdm.jqgufenzy.top

Py:   ",".join(items)
来源：http://pyb.jianghu66.top

PHP:  implode(",", $items);
来源：http://bbc.xuanzx.com

JS:   items.join(",")
来源：http://yug.hongshengwenyu.top

TS:   items.join(",")
来源：http://fiu.jyoumei.cn

Java: String.join(",", items)
来源：http://qyj.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://yid.cashguo.top

Ruby: items.join(",")
来源：http://wol.xuanzx.com

C#:   string.Join(",", items)
来源：http://cfo.gzhubu.top

[E09] 去除所有空白字符
来源：http://awi.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://edn.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sbo.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://hxa.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://vya.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://msg.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rji.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://dad.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://azk.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://fbn.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://snj.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wfb.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://bwz.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://zac.xuanzx.com

Java: String.format("%03d", 7)
来源：http://bqj.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xmt.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wbl.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wmm.yonumen.top

[E11] 反转字符串
来源：http://fap.chenlongwang.top

Py:   s[::-1]
来源：http://lrp.fktsv.cn

PHP:  strrev($s);
来源：http://nst.ivvv.top

JS:   [...s].reverse().join("")
来源：http://rrb.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://lym.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uej.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gzu.jinqigfzy.top

Ruby: s.reverse
来源：http://vwv.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://jhi.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://qto.cheryme.top

Py:   s.count("a")
来源：http://umk.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://ugq.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://lxe.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://bhg.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://avf.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://pet.andypj.xyz

Ruby: s.count("a")
来源：http://pod.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://naq.jlsjyb.cn

[E13] 逐字符遍历
来源：http://nwp.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://xej.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jja.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://okj.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://men.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iph.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wha.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hpp.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ntm.ydzc1.top

[E14] URL 编码与 Base64
来源：http://pcb.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://chs.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sfx.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ozr.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xlj.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://prq.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wcl.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://slg.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nwd.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://pyx.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://lnr.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wcj.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jkf.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lde.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jus.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbu.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ihy.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hzv.guowangkeji.top

[E16] 数字千分位
来源：http://ank.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://qps.iojbl.cn

PHP:  number_format(1234567);
来源：http://vyu.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mrw.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bhr.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jee.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cxa.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zuu.yj202588.top

C#:   1234567.ToString("N0")
来源：http://eia.cucudq.cn

[E17] 首字母大写
来源：http://dpw.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sls.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://guy.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lzg.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gbe.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://azc.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oji.pycfn.com

Ruby: s.capitalize
来源：http://lyo.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ctr.vehdjk.com

[E18] 模板占位符替换
来源：http://whb.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iaq.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hhm.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dmi.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rwl.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zhd.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xha.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hvy.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://esr.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://kkl.jqgufenzy.top

Py:   s.splitlines()
来源：http://kup.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rzi.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://xev.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://tey.yfazqb.com

Java: s.lines().toList()
来源：http://kzl.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://uas.chenlongwang.top

Ruby: s.lines
来源：http://nhg.zhengqikj.top

C#:   s.Split('\n')
来源：http://xvy.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://nlt.fehbvm.com

Py:   if not s:
来源：http://yia.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yvy.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gwo.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://apw.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://byw.mhx1999.top

Go:   if s == "" {}
来源：http://kgh.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://ddi.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fwe.cheryme.top

[E21] 超长截断加省略号
来源：http://tlj.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gkb.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://avm.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fbc.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axg.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mqi.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://dnx.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ton.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ojk.hammf.cn

[E22] 字节长度与字符长度
来源：http://vaw.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rzt.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://foh.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fbh.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dge.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xzg.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lhv.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://uvy.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://etz.cqqwz.cn

================================================================================
来源：http://dgh.dianchejie.cn

F. 文件与目录
来源：http://amc.cheryme.top

================================================================================
来源：http://gfl.ctjpmb.com

[F01] 读取整个文件
来源：http://gml.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hjk.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://qqe.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xmo.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hhq.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xdl.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rjy.316326.xyz

Ruby: File.read("a.txt")
来源：http://rgx.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://rek.shzxlz.cn

[F02] 逐行读取文件
来源：http://kpw.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zev.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uxm.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://orm.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hpg.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tgc.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qyx.52xcode.cn


<!-- 参考信息 -->