代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://xpu.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kxb.redwolf501.top

TS:   Math.max(...arr);
来源：http://jpb.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://cqk.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qcy.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://zhq.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://tzg.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://hlu.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ovc.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://jai.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zan.gzhubu.top

TS:   nested.flat();
来源：http://wou.fehbvm.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kaa.meibo888.top

Go:   // 手写双层循环
来源：http://ldf.zhixingplan.top

Ruby: nested.flatten
来源：http://bvl.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xyn.ctjpmb.com

[D19] 按字段分组
来源：http://edq.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dta.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cyt.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ydn.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wbn.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://czc.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://qpc.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://faz.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dhj.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://ftc.fengsongda.top

Py:   Counter(arr)
来源：http://phm.vehdjk.com

PHP:  array_count_values($arr);
来源：http://bkq.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hol.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jny.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ifs.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://jgb.hnxiangtu.top

Ruby: arr.tally
来源：http://blh.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hfc.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://pvi.chenjidiqi.icu

Py:   x in arr
来源：http://bit.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://erv.dianchejie.cn

JS:   arr.includes(x)
来源：http://apo.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://lps.yueranfly.top

Java: list.contains(x)
来源：http://qqs.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://koq.hfpthk.cn

Ruby: arr.include?(x)
来源：http://rxu.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://vhb.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://pqk.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://usc.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ywx.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://red.yuxming.cn

TS:   [...arr];
来源：http://vlj.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://pid.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yfx.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://nlr.nanxinkj.top

C#:   new List<int>(list);
来源：http://lqn.bbcook.cn

[D23] reduce 累积计算
来源：http://lmk.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mkq.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zyn.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfp.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ejy.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://znv.ybcxt.top

Go:   // 手写循环
来源：http://uih.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://njn.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ihe.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://xyr.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oks.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sfy.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gnk.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ytq.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vhy.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wkw.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://btr.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jyr.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://ewg.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sar.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hxr.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jdi.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hty.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cdo.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zwg.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pwb.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ved.zdqjudy.top

[D26] 数组转字符串
来源：http://cns.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://tnh.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://zqs.xinyue.icu

JS:   arr.join(", ")
来源：http://wlk.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://hrn.andypj.xyz

Java: String.join(", ", list)
来源：http://uxi.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://cpq.gogol.net.cn

Ruby: arr.join(", ")
来源：http://msa.andypj.xyz

C#:   string.Join(", ", list)
来源：http://xim.dashuyun.cn

================================================================================
来源：http://jiz.vqdsnc.cn

E. 字符串处理
来源：http://uex.yj20258.top

================================================================================
来源：http://iet.havefunace.top

[E01] 拼接字符串
来源：http://bot.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nqn.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://git.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fns.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nkd.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qdy.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://acw.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jfw.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yge.0kj1m.cn

[E02] 重复字符串
来源：http://fgt.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://fzq.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://owg.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://nxu.hcnkem.com

TS:   "ab".repeat(3)
来源：http://nhz.fzhhl.top

Java: "ab".repeat(3)
来源：http://zks.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://wpz.jianghu66.top

Ruby: "ab" * 3
来源：http://alz.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bho.fanxiaobao.xyz

[E03] 截取子串
来源：http://skf.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qzc.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://crc.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pkr.smart0.xyz

TS:   s.slice(1, 4)
来源：http://ilm.shuidangran.top

Java: s.substring(1, 4)
来源：http://eee.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vax.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://mpp.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://vni.xinyue.icu

[E04] 查找子串位置
来源：http://oju.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://txp.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://iit.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fls.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://hzg.cheryme.top

Java: s.indexOf("x")
来源：http://jpu.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://mlt.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://hwu.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://nnk.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ips.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pqi.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cwx.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zbw.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dvm.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wnk.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cbk.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mcy.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zrd.chenzaomai.com

[E06] 替换子串
来源：http://eul.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fco.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ipf.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xon.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://srz.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ues.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gix.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vzn.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://ljy.chenzaomai.com

[E07] 按分隔符拆分
来源：http://hic.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yhc.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cwx.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://tna.zhengqikj.top

TS:   s.split(",")
来源：http://gfx.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tbg.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yax.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://pda.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bcn.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://nco.feifeiyinyue.top

Py:   ",".join(items)
来源：http://fpw.jyoumei.cn

PHP:  implode(",", $items);
来源：http://hvn.nanxuanxn.top

JS:   items.join(",")
来源：http://arx.wangdashe.top

TS:   items.join(",")
来源：http://tlv.jinqigfzy.top

Java: String.join(",", items)
来源：http://asx.guannengcc.top

Go:   strings.Join(items, ",")
来源：http://exe.guowangkeji.top

Ruby: items.join(",")
来源：http://ffc.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://fya.haohaochexian.top

[E09] 去除所有空白字符
来源：http://sae.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fow.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xbd.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://lky.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://uhx.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://pwv.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hkd.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bky.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tfz.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://lgr.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sry.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wmq.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://akn.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://dqg.iojbl.cn

Java: String.format("%03d", 7)
来源：http://mnb.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wxl.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rbs.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://izw.iojbl.cn

[E11] 反转字符串
来源：http://xsk.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://zuy.yangfankeji.com

PHP:  strrev($s);
来源：http://jmy.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://gve.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://ftn.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zwd.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://thp.jqgfzy.top

Ruby: s.reverse
来源：http://swo.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://ccm.yueranfly.top

[E12] 统计某字符出现次数
来源：http://pqy.tian-w.cn

Py:   s.count("a")
来源：http://tfg.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://brj.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://emr.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://rpo.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://web.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://aub.aibaodan.cn

Ruby: s.count("a")
来源：http://mho.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://qwy.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://fcw.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://mpd.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vzt.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://geb.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dss.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dip.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ksy.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fda.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hgp.xylfe.cn

[E14] URL 编码与 Base64
来源：http://opv.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zer.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://boy.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vzi.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://imm.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iji.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qdn.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zcx.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pdc.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://qof.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uza.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xsr.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vre.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://pci.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fjo.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hee.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lir.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sid.bbcook.cn

[E16] 数字千分位
来源：http://lvw.andypj.xyz

Py:   f"{1234567:,}"
来源：http://ixe.ppjwa.cn

PHP:  number_format(1234567);
来源：http://mft.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ven.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bqk.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dyv.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://msy.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xni.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://fvj.gaohongyu789.top

[E17] 首字母大写
来源：http://vhy.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eks.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://myr.fanxiaobao.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vqv.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dja.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://srd.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yai.jlsjyb.cn

Ruby: s.capitalize
来源：http://bhk.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ucx.birdmap.top

[E18] 模板占位符替换
来源：http://wik.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ovv.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://onb.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ysc.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://juh.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ojp.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rdu.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ozm.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://twh.52xcode.cn

[E19] 多行文本按行拆分
来源：http://xbx.epnwcf.com

Py:   s.splitlines()
来源：http://eni.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nnc.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://ycs.jinyuanbaomall.cn

TS:   s.split(/\r?\n/)
来源：http://rxh.meibo888.top

Java: s.lines().toList()
来源：http://qho.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://ljw.fanxiaobao.xyz

Ruby: s.lines
来源：http://kve.pycfn.com

C#:   s.Split('\n')
来源：http://vbv.sweek.top

[E20] 判断字符串是否为空
来源：http://hja.yj20258888.top

Py:   if not s:
来源：http://cui.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ktj.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zpo.mhx1999.top

TS:   if (s === "") {}
来源：http://wzi.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://nbz.jlsjyb.cn

Go:   if s == "" {}
来源：http://mpj.sysykeji.top

Ruby: if s.empty?
来源：http://zkt.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hbc.ydzc1.top

[E21] 超长截断加省略号
来源：http://blk.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vvw.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cao.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmi.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aom.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hbw.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://qcw.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uxb.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zvk.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://mxp.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oaz.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zdq.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqw.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cyb.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bvc.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sbm.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://ogb.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iec.vqdsnc.cn

================================================================================
来源：http://rfp.dashuyun.cn

F. 文件与目录
来源：http://ggf.jinqigfzy.top

================================================================================
来源：http://wpd.fzhhl.top

[F01] 读取整个文件
来源：http://ibg.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gls.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://ylz.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tol.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://atf.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://zae.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ggk.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://len.yvedp.cn


<!-- 参考信息 -->