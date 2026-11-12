代发 wailian999

C#:   list.Distinct().ToList()
来源：http://xwe.gotoacloud.top

[D16] 求和与平均值
来源：http://wln.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kvj.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nhc.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://spf.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wuo.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://umx.yueranfly.top

Go:   // 手写循环累加
来源：http://fnj.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://azf.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://lvn.zhengqikj.top

[D17] 最大值与最小值
来源：http://rcl.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://xxs.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://ebm.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rla.meibo888.top

TS:   Math.max(...arr);
来源：http://mna.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yiy.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fcd.birdmap.top

Ruby: arr.max;  arr.min
来源：http://bax.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://wqu.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://pnt.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sow.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://yhx.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://arb.hesvh.cn

TS:   nested.flat();
来源：http://ywb.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gfq.ivvv.top

Go:   // 手写双层循环
来源：http://kye.sysykeji.top

Ruby: nested.flatten
来源：http://yyh.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://btx.tian-w.cn

[D19] 按字段分组
来源：http://szi.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eep.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jgf.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gsj.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bbf.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcp.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://ynt.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://les.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ife.tanke756.top

[D20] 统计每个元素出现次数
来源：http://dnk.hywenlv.cn

Py:   Counter(arr)
来源：http://fwc.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://lpe.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://smh.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdl.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vib.yj20258888.top

Go:   // 手写 map[T]int
来源：http://oem.nwbrower.top

Ruby: arr.tally
来源：http://mkw.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ids.meibo888.top

[D21] 判断是否包含某元素
来源：http://jrn.zhengqikj.top

Py:   x in arr
来源：http://wlz.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://kuz.zdqjudy.top

JS:   arr.includes(x)
来源：http://zto.shzxlz.cn

TS:   arr.includes(x)
来源：http://lfh.yj20258888.top

Java: list.contains(x)
来源：http://sit.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://yum.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://bbk.yvedp.cn

C#:   list.Contains(x)
来源：http://zht.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://xer.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xnp.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ray.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://axb.jqgufenzy.top

TS:   [...arr];
来源：http://kho.jqgfzy.top

Java: new ArrayList<>(list);
来源：http://eqg.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://grn.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://enp.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://ksp.sjlbkw.cn

[D23] reduce 累积计算
来源：http://nlu.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://foc.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hpz.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awb.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wki.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qcn.shangyingyoupin.top

Go:   // 手写循环
来源：http://bbh.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cxm.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fbk.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://hzi.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cyd.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gbm.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qyv.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://avn.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://omb.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jdx.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://unk.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yoy.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://rgj.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ygp.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ekq.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cwv.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://owv.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vzh.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xgk.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mhd.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bpm.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://txq.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://ksl.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://ctw.daxiang520.top

JS:   arr.join(", ")
来源：http://gpf.vqdsnc.cn

TS:   arr.join(", ")
来源：http://tmm.xziqi.cn

Java: String.join(", ", list)
来源：http://txd.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://cyw.jianghu66.top

Ruby: arr.join(", ")
来源：http://lrd.bbcook.cn

C#:   string.Join(", ", list)
来源：http://xwj.yuxming.cn

================================================================================
来源：http://aed.fehbvm.com

E. 字符串处理
来源：http://xtz.ybcxt.top

================================================================================
来源：http://fjo.tianlin.xyz

[E01] 拼接字符串
来源：http://hmo.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tnl.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hyy.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xnd.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://juc.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jue.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rlg.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sxh.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zxa.meibo888.top

[E02] 重复字符串
来源：http://kso.meibo888.top

Py:   "ab" * 3
来源：http://xfp.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://uku.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://wra.yongpay.top

TS:   "ab".repeat(3)
来源：http://roe.xuanzx.com

Java: "ab".repeat(3)
来源：http://cgm.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://gck.yuxming.cn

Ruby: "ab" * 3
来源：http://rcu.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sfv.jiagoushi.top

[E03] 截取子串
来源：http://ozu.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://don.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ybz.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qwk.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://bdn.daxiang520.top

Java: s.substring(1, 4)
来源：http://cbs.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qah.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://mnh.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://jaa.iojbl.cn

[E04] 查找子串位置
来源：http://psa.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://yxx.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://ena.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lsq.daxiang520.top

TS:   s.indexOf("x")
来源：http://ejx.fengsongda.top

Java: s.indexOf("x")
来源：http://whb.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://qtv.nwbrower.top

Ruby: s.index("x")
来源：http://lcy.epnwcf.com

C#:   s.IndexOf("x")
来源：http://dcq.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iph.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hze.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sdx.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mob.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sxv.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mry.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aaw.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rpa.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iii.zhiwuduotai.top

[E06] 替换子串
来源：http://irn.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kvm.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://uib.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wnm.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://cul.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oey.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bxp.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://apm.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://gyv.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://bth.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zda.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hql.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ask.xylfe.cn

TS:   s.split(",")
来源：http://bal.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bex.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cvf.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://cdp.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tyo.havefunace.top

[E08] 数组按分隔符合并
来源：http://yqf.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://ncq.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://dvx.chenjidiqi.icu

JS:   items.join(",")
来源：http://myl.xinyue.icu

TS:   items.join(",")
来源：http://unx.yuanzhike.top

Java: String.join(",", items)
来源：http://xbl.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://cny.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://ntm.jinqigufen.top

C#:   string.Join(",", items)
来源：http://ryr.sufxvd.cn

[E09] 去除所有空白字符
来源：http://nmu.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wuh.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gbx.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://wog.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://cuc.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://rut.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nkp.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://bbl.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tbc.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://wgs.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qjk.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tki.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://hdw.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://ymy.yvedp.cn

Java: String.format("%03d", 7)
来源：http://phq.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kli.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ipt.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ufi.fzhhl.top

[E11] 反转字符串
来源：http://eco.xziqi.cn

Py:   s[::-1]
来源：http://pel.nanxinkj.top

PHP:  strrev($s);
来源：http://bdg.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://fpk.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://qlz.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mfj.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kwx.quarkkingdee.top

Ruby: s.reverse
来源：http://xvh.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://fls.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://qcs.ydzc1.top

Py:   s.count("a")
来源：http://wzo.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://wbw.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://kld.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://hfn.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lzl.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://amw.jiagoushi.top

Ruby: s.count("a")
来源：http://foz.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://tci.ydzc1.top

[E13] 逐字符遍历
来源：http://jrg.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://nmo.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bsj.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ize.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://frl.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://izz.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://muu.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ifb.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rya.pycfn.com

[E14] URL 编码与 Base64
来源：http://kbq.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hdn.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ojq.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qjl.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jqq.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ntp.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ipv.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wkz.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zjl.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://szm.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bzp.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nvw.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mfa.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://igc.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uhf.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ftg.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zug.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tcc.hammf.cn

[E16] 数字千分位
来源：http://fqg.hesvh.cn

Py:   f"{1234567:,}"
来源：http://rlv.yfazqb.com

PHP:  number_format(1234567);
来源：http://tbm.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fnz.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ylq.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zyi.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qei.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zmy.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://ujr.xuetiantiany.cn

[E17] 首字母大写
来源：http://fzg.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://app.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://fxr.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yrm.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yao.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ulv.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yon.hcnkem.com

Ruby: s.capitalize
来源：http://sma.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fpj.iojbl.cn

[E18] 模板占位符替换
来源：http://dou.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qyy.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ukx.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://znq.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yau.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wcu.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hig.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uvh.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yyl.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://hlm.ehwqpu.com

Py:   s.splitlines()
来源：http://eer.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ukj.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://khn.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://zob.sjlbkw.cn

Java: s.lines().toList()
来源：http://ldy.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://gol.jlsjyb.cn

Ruby: s.lines
来源：http://aet.dianchejie.cn

C#:   s.Split('\n')
来源：http://njl.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://fnq.feifeiyinyue.top

Py:   if not s:
来源：http://kzh.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uqg.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uls.zhijiandao.cn

TS:   if (s === "") {}
来源：http://ahu.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://dvo.52xcode.cn

Go:   if s == "" {}
来源：http://ujt.chenzaomai.com

Ruby: if s.empty?
来源：http://joi.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uzx.tarul.cn

[E21] 超长截断加省略号
来源：http://vgo.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xwh.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qqv.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iin.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kji.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eua.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://uni.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://txp.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zvn.316326.xyz

[E22] 字节长度与字符长度
来源：http://upp.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://akf.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cuq.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bxt.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sub.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ezz.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xky.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://hgf.ehwqpu.com


<!-- 参考信息 -->