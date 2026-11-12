代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pdx.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tkn.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mll.guannengcc.top

Go:   // 手写循环累加
来源：http://ivi.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dcb.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://htk.jqgufenzy.top

[D17] 最大值与最小值
来源：http://efk.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://eui.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://iil.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jss.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://jex.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://leo.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xvd.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://ril.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://tyi.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://vmf.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zoi.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://zms.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://syj.kuanghao11.cn

TS:   nested.flat();
来源：http://ifi.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://het.yangfankeji.com

Go:   // 手写双层循环
来源：http://xkj.mhx1999.top

Ruby: nested.flatten
来源：http://vss.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uta.nwbrower.top

[D19] 按字段分组
来源：http://ftn.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xsh.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pva.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vhy.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ypy.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lvb.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://rjc.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jjf.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ykc.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://ero.havefunace.top

Py:   Counter(arr)
来源：http://biz.ydzc1.top

PHP:  array_count_values($arr);
来源：http://row.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://prm.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cmf.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hhh.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://bed.52xcode.cn

Ruby: arr.tally
来源：http://nyh.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fyk.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://xta.pycfn.com

Py:   x in arr
来源：http://wuh.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://yxe.vqdsnc.cn

JS:   arr.includes(x)
来源：http://dzg.kuanghao11.cn

TS:   arr.includes(x)
来源：http://rhl.yj202588.top

Java: list.contains(x)
来源：http://prs.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://vgr.9152youxi.cn

Ruby: arr.include?(x)
来源：http://xlc.ybcxt.top

C#:   list.Contains(x)
来源：http://vkt.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://ojb.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oai.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mfs.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://anf.sysykeji.top

TS:   [...arr];
来源：http://arw.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://yaj.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://wal.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://tbz.yfazqb.com

C#:   new List<int>(list);
来源：http://voq.havefunace.top

[D23] reduce 累积计算
来源：http://mua.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wvk.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ofz.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://csu.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blr.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://lui.zhengqikj.top

Go:   // 手写循环
来源：http://zto.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vsn.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xnk.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://nqb.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ghl.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xuw.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ilr.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yef.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sde.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://etk.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://byl.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://puy.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://pei.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mjx.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://chs.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jzo.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dbt.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nqk.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tzu.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qsf.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://euc.fehbvm.com

[D26] 数组转字符串
来源：http://guv.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://qyw.316326.xyz

PHP:  implode(", ", $arr);
来源：http://kpk.ydzc1.top

JS:   arr.join(", ")
来源：http://odv.aizwys.cn

TS:   arr.join(", ")
来源：http://dkn.ybcxt.top

Java: String.join(", ", list)
来源：http://ezt.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://mqf.cucudq.cn

Ruby: arr.join(", ")
来源：http://hfd.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://fho.ehwqpu.com

================================================================================
来源：http://cds.jinghuilouyu.cn

E. 字符串处理
来源：http://mbp.ppjwa.cn

================================================================================
来源：http://mww.cashguo.top

[E01] 拼接字符串
来源：http://cdw.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blr.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://urp.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://flv.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wuh.zycfv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://epb.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rxg.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yca.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xda.0kj1m.cn

[E02] 重复字符串
来源：http://glf.ydzc1.top

Py:   "ab" * 3
来源：http://bip.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://qpd.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://gmb.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://ifa.sufxvd.cn

Java: "ab".repeat(3)
来源：http://isy.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://taa.nanxuanxn.top

Ruby: "ab" * 3
来源：http://owh.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oij.tarul.cn

[E03] 截取子串
来源：http://znh.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uej.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fhi.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://smm.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://aoi.hnqzz.top

Java: s.substring(1, 4)
来源：http://krd.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dtk.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jtb.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://udr.vehdjk.com

[E04] 查找子串位置
来源：http://xyv.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://jbg.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://wle.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://onz.yj20258.top

TS:   s.indexOf("x")
来源：http://syj.shzxlz.cn

Java: s.indexOf("x")
来源：http://qlx.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://pou.yvedp.cn

Ruby: s.index("x")
来源：http://vff.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://xfi.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ltb.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ivn.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cno.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://emq.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cvq.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lmj.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ylc.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ftm.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jwf.shanyushiyangtech.top

[E06] 替换子串
来源：http://pmb.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vsb.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://kzy.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jby.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://fbk.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gok.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://znm.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://drs.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://joj.vehdjk.com

[E07] 按分隔符拆分
来源：http://nrb.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://out.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fkw.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gbx.xylfe.cn

TS:   s.split(",")
来源：http://gkt.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aua.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxv.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://uto.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dfe.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://lnw.zhiwuduotai.top

Py:   ",".join(items)
来源：http://jev.cheryme.top

PHP:  implode(",", $items);
来源：http://tua.tian-w.cn

JS:   items.join(",")
来源：http://ksq.yonumen.top

TS:   items.join(",")
来源：http://aap.hnqzz.top

Java: String.join(",", items)
来源：http://xbz.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://gwm.yueranfly.top

Ruby: items.join(",")
来源：http://koq.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://ipg.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://zab.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://whc.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lhb.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://zgm.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://wsr.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://tuh.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yrq.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://gza.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://smo.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://vri.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oga.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iew.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://gmg.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://yvt.bbcook.cn

Java: String.format("%03d", 7)
来源：http://rpq.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jfw.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ubz.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bbt.cheryme.top

[E11] 反转字符串
来源：http://qsw.epnwcf.com

Py:   s[::-1]
来源：http://rsu.yuanzhike.top

PHP:  strrev($s);
来源：http://hba.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://mos.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://smp.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lbs.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rtl.tianlin.xyz

Ruby: s.reverse
来源：http://wkb.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://lxt.hammf.cn

[E12] 统计某字符出现次数
来源：http://qvy.c1oappe.top

Py:   s.count("a")
来源：http://soh.yonumen.top

PHP:  substr_count($s, "a");
来源：http://znq.tian-w.cn

JS:   s.split("a").length - 1
来源：http://dba.tian-w.cn

TS:   s.split("a").length - 1
来源：http://gsq.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rwo.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://cec.hammf.cn

Ruby: s.count("a")
来源：http://xfq.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://ieu.pycfn.com

[E13] 逐字符遍历
来源：http://jrw.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://voo.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jxf.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://bou.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hay.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jjg.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://khv.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ldc.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tfs.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://ptr.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://syn.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fdo.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://djr.hongshengwenyu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://shi.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gpo.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cpa.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hud.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hbg.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://wye.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ajs.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lme.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://amf.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wjn.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gcc.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://epc.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pqy.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://myf.yj20258.top

[E16] 数字千分位
来源：http://obt.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://ecv.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://key.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://emn.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dvm.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://man.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yyl.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xpl.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://qob.vehdjk.com

[E17] 首字母大写
来源：http://bni.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ruu.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qpk.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://exa.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fcg.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zwi.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uvl.gzhubu.top

Ruby: s.capitalize
来源：http://mrn.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mro.fktsv.cn

[E18] 模板占位符替换
来源：http://sol.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bcg.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tib.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zvp.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dvc.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ybu.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jqm.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hdb.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mpd.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://hss.ydzc1.top

Py:   s.splitlines()
来源：http://ufi.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jmb.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://fks.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://akw.jinqigfzy.top

Java: s.lines().toList()
来源：http://tcb.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://fjc.mhx1999.top

Ruby: s.lines
来源：http://eli.cheryme.top

C#:   s.Split('\n')
来源：http://lmp.birdmap.top

[E20] 判断字符串是否为空
来源：http://aqv.guannengcc.top

Py:   if not s:
来源：http://gsu.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://okx.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://obp.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://riq.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://udl.aizwys.cn

Go:   if s == "" {}
来源：http://zhf.tian-w.cn

Ruby: if s.empty?
来源：http://kxf.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yjb.mhx1999.top

[E21] 超长截断加省略号
来源：http://pkm.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ytz.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tdp.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://unm.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://enr.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yqt.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://fpw.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iad.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nlq.fengsongda.top

[E22] 字节长度与字符长度
来源：http://pyy.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wbb.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddk.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvd.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzf.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://niz.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kgt.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://cyn.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bqn.havefunace.top

================================================================================
来源：http://ayk.pengpengdd.cyou

F. 文件与目录
来源：http://qts.jinqigufen.top

================================================================================
来源：http://jhn.hfpthk.cn


<!-- 参考信息 -->